# Question 3

> Create a file in your system. Whenever a someone performs some action(read, write, execute) on that file, the event should be logged somewhere

To track a file in the system we can use Auditd, which is a monitoring tool used for auditing activity like authentications, failed cryptographic operations, abnormal terminations, program execution, and SELinux modifications. 

CentOS ships with Auditd, but Ubuntu does not so to install it we use the command:

```
~ sudo apt install auditd
```

Now to monitor a file at the location **/home/prajesh/checkme/watching.txt** we edit the auditd config file at location **/etc/audit/rules.d/audit.rules** to add the rules for *File Access monitoring*:

```
-w /home/Prajesh/checkme/watching.txt -p rwx -k watch_file
```

Here the format of the rule for File Access monitoring is

```
-w <path/to/file/location> -p <permissions/to/monitor> -k <key_name>
```

So now any changes in the file will be logged in the logs file in the location **/var/log/audit/audit.log.**

We can search through the log file using **ausearch** tool as such:

```
~ ausearch -k watch_file
```

![log](screenshots/Screenshot%202021-11-28%20161357.png)