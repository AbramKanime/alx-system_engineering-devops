![](https://t3.ftcdn.net/jpg/04/92/09/72/240_F_492097246_yagE8x9Uk8M9IekPy7GBuE0x1Uoa7esD.jpg)
## Issue Summary:
![](https://www.cienotes.com/wp-content/uploads/2019/07/summaryblackboard.jpg)
On January 20, 2024, between 11:00 AM to 1:00 PM WAT, users experienced a service outage on our e-commerce platform. During this time, the platform was completely down, preventing users from accessing the website, browsing products, or making purchases. Approximately 75% of our users were affected by this outage.

## Root Cause:
![](https://blog.systemsengineering.com/hs-fs/hubfs/blog-files/Root%20Cause.jpg?width=600&name=Root%20Cause.jpg)
The root cause of the outage was identified as a critical failure in the load balancer. This failure caused a high volume of traffic to be redirected to a single server, overloading it and causing it to crash. The load balancer failed to recognize this issue and continued to direct traffic to the overloaded server.

## Timeline:
![](https://www.ncbar.org/wp-content/uploads/2022/02/Timeline-Visual-300x145.png)
- 11:00 AM WAT: The outage was first detected through monitoring alerts.
- 11:05 AM WAT: The engineering team was notified of the issue and began investigating.
- 11:10 AM WAT: The team identified the load balancer as a possible root cause and began investigating.
- 11:30 AM WAT: The team identified the overloaded server as the root cause and attempted to restart it.
- 11:45 AM WAT: After restarting the server, the team realized that the issue persisted and escalated the incident to the senior engineering team.
- 12:00 PM WAT: The senior engineering team took over the incident and identified the load balancer as the root cause.
- 12:30 PM WAT: The senior engineering team replaced the load balancer and verified that the platform was back online.
- 1:00 PM WAT: The platform was confirmed to be fully operational.

## Misleading Investigation/Debugging Paths:
Initially, the team suspected that the server was overloaded due to a sudden spike in traffic or a DDoS attack. They spent time investigating traffic patterns and examining logs, but these efforts proved to be misleading. This delayed the identification of the root cause and prolonged the outage.

## Incident Escalation:
The incident was escalated to the senior engineering team after the initial attempts to resolve the issue were unsuccessful.

## Resolution:
The senior engineering team replaced the load balancer with a new one and verified that the platform was back online. They also implemented additional monitoring to prevent similar issues from occurring in the future.

## Corrective and Preventative Measures:
- Implement more robust monitoring for the load balancer to detect failures earlier.
- Implement automatic failover mechanisms to prevent a single server from being overloaded.
- Increase redundancy in the infrastructure to prevent single points of failure.
- Conduct a thorough review of the incident to identify areas for improvement in incident response procedures.

In conclusion, the e-commerce platform outage on January 20, 2024, was caused by a critical failure in the load balancer, which resulted in an overloaded server and prevented users from accessing the platform. The incident was resolved by replacing the load balancer and implementing additional monitoring and failover mechanisms. To prevent similar incidents from occurring in the future, the team will implement more robust monitoring, increase redundancy, and conduct a thorough review of incident response procedures.
