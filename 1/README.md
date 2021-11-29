# Question 1

> List some logging and visualization tools available in the market with the preferred scenario to use one over other.

Logs are crucial data about users, traffic, performance and security related aspects of a distributed environment. Visualizing these logs and interpreting it in an understandable way is as much important. Some of the tools that are available now for logging and visualization are listed below

- ELK Stack
- Graylog
- Splunk
- Sumo Logic
- Loggly

#### ELK Stack
ELK stack is an open-source project made up of many different tools for application data analysis and visualization. Logstash, specifically, was made for the collection and management of log files. Beyond log aggregation, it includes ElasticSearch for indexing and searching through data and Kibana for charting and visualizing data. Together they form a powerful log management solution.

**When to use it**: If you want an open-source tool. If you’re interested in implementing the entire Elastic stack or at least see value separately in using ElasticSearch or Kibana and want the interactive benefits that come from combining these tools.

### GrayLog
Graylog is an open-source log analyzer backed by MongoDB as well as ElasticSearch (similar to Logstash) for storing and searching log errors. It’s mainly focused on helping developers detect and fix errors in their apps, but they’ve also released an official enterprise-ready platform.

**When to use it**: Graylog is more targeted towards developers than other open-source log management tools. Plus, if you want a log management tool that aims to be both enterprise-ready and is open source, Graylog definitely deserves to be in the mix with Elastic/Logstash.

### Splunk
Splunk is the biggest tool in the log management space. It’s well-established, full-featured, and enterprise-class. It’s unique in this space as an on-premises tool (although they have come out with a Cloud version as well).

**When to use it**: Enterprise companies with lots of feature needs and a variety of data that needs analyzing.

### Sumo Logic
Sumo Logic was founded as a SaaS version of Splunk, going so far as to imitate some of Splunk’s features and visuals early on. Since then, Sumo Logic has developed into a full-fledged enterprise-class log management solution in its own right. Sumo Logic is the most enterprise-focused of the cloud-native log analyzers.

**When to use it**: If you’re an enterprise-type company but are willing to sacrifice some features for the benefits of SaaS, Sumo Logic is worth exploring. It’s also good if you have a strong focus on security. It’s not just developer-oriented as a tool either, with benefits for security teams and business purposes.

### Loggly
Loggly is a robust log analyzer, focusing on simplicity and ease of use. It’s targeted for developers and DevOps – making it less enterprise-focused.

**When to use it**: Primary use cases are for troubleshooting and customer support scenarios. It’s a good tool for a DevOps team.

### PaperTrail
PaperTrail is a simple way to look and search through logs from multiple machines, in one consolidated easy-to-use interface. It’s a SaaS tool designed to enhance the logs you already collect or generate.

**When to use it**: If you want a simple and straightforward tool without lots of extra bells and whistles. If you want a stripped down and basic log analyzer that is good for looking at log files in aggregation and doesn’t try to be anything more.
