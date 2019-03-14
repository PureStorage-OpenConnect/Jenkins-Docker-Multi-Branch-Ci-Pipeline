# Devloping Software In Teams

![team development](https://user-images.githubusercontent.com/15145995/46342585-0556b380-c633-11e8-96cf-18c34d17c717.PNG)
---
# Avoiding External Port Clashes

In software development speak, "Mutual exclusion" is a means of ensuring that only one thread or process can access a specific code path at a time. We see this in multiple places through the SQL Server database engine:

- Locks
- Latches
- Spinlocks

In this specific example we need to ensure that when spinning up multiple containers, more than one container does not attempt to grab the same external port on the host
We achieve this using the lockable resource plugin for Jenkins, the section that begins with "lock (" is all important here:

![lockable resource](https://user-images.githubusercontent.com/15145995/46342829-b1989a00-c633-11e8-8054-07b23a202d13.PNG)
---
# Points Of Interest

![points of interest](https://user-images.githubusercontent.com/15145995/46342943-16ec8b00-c634-11e8-8b40-721b2edf52f4.PNG)
