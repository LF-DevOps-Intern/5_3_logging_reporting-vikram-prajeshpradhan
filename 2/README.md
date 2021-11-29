# Question 2

> Mention 10 best practices when logging. Why is log formatting necessary?

Some Best Practices when logging is listed below.

- **Log at the Proper Level**
Not all events are equally important for troubleshooting or network monitoring, and being able to differentiate severe ones from irregular or normal logs is critical. Logging levels should be a part of all logs for all devices, including statements such as FATAL, ERROR, WARN, INFO, DEBUG, TRACE, ALL, or OFF.

- **Find the Middle Ground in Detail**
When configuring what kind of information your logs provide, you need to find the middle ground in the amount of detail your log messages show.

- **Logging Standard**
Logs needs to be consistent so using a logging standard is preferrable. Ensure all logs show the timestamp and the names of the host and logger. Other valuable information can include event or user ID, application version, and metrics.

- **Log in Machine Parse able Format**
Log entries are really good for humans but very poor for machines. Sometimes it is not enough to manually read log files, you need to perform some automated processing. *This is also the reason why log formatting is necessary.*

- **Meaningful Log Messages**
As logs are the first thing to look into in the time of emergency, it needs to be simple and meaningful which in turn helps understand what happened.

- **Add Context**
Without proper context, those messages are only noise, they don’t add value and consume space that could have been useful during troubleshooting.

- **NOT logging Sensitive information**
Sensitive information like passwords, credit card information and social security numbers must not be logged. It may expose certain vulnerabilities to the system.

- **Anticipate common scenarios**
Logging with some common scenarios in mind ensures the logs provide direct value to your organization. Logs aren’t just for incident response. Logs can help with other parts of your business, such as performance profiling or gathering statistics.

- **Log In English**
English means your messages will be in logged with ASCII characters. If your message uses a special charset or even UTF-8, it might not render correctly at the end, but worst it could be corrupted in transit and become unreadable.
