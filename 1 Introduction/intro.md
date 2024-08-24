# What is Dynatrace?
```sh
It's a one stop analytics and automation platform to achieve unified observability and security.

observability:  It is the ability of a system to process large amounts of data in form of logs and metrics,
and provide actionable insights and suggestions based on it

security: It is a set of measures and a set of steps that companies take to protect its data and
its user base from unauthorized access from the outside

```
## High Level Architecture
```sh
1. OneAgent
2. PurePath
3. GrailDB
4. AutomationEngine
```
### OneAgent
```sh
1. The OneAgent in Dynatrace is a software that you install on your servers, virtual machines, or containers.
2. Its job is to automatically monitor everything that's happening on those systems.
3. OneAgent as a smart assistant that quietly sits on your servers and keeps an eye on everything—like how your
   applications are running, how your servers are performing, and if there are any issues or slowdowns.
4. It collects different metrics on various aspects of your hosts, where your host can be just one server, or
   a cluster, and it monitors hardware, operating system and application processes
4. It gathers all this information and sends it back to Dynatrace, where you can see it in a dashboard
```
### PurePath
```sh
1. PurePath in Dynatrace is a feature that traces the entire journey of a single user request or
   transaction as it flows through different components of your application, from the user's interaction to
   the backend services and databases.
2. PurePath captures and records every step of this journey, showing you how long each step takes,
   which parts of the system are involved, and where any slowdowns or errors occur. It helps developers and IT teams
   to understand exactly how the system is working and where they might need to fix or optimize something
3. It's feature provided by Dynatrace and enabled through the OneAgent installed on server that needs to be monitored
```
### GrailDB
```sh
1. GrailDB is a database designed explicitly for observability and security
2. Grail DB as a super-organized storage room that collects all the performance data, logs, and traces that Dynatrace
   gathers from your applications and servers.
3. This data could be things like how fast your website is loading, any errors that are happening, or how your servers
   are performing.
4. Grail DB not only stores this information but also makes it easy to search through, analyze, and understand all of it.
5. schema on read:
6. Indexless
```
