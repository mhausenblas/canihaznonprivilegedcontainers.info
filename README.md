# Non-privileged containers FTW!

Did you know that running containers with user `root` not only a bad practice but really is a security risk. You might not care when launching a single container on your laptop, but in the context of container orchestrators such as Kubernetes, this is a real problem. This site tries to explain the issue, collects data and reference material and ultimately provide you with tooling to change the status quo. We can do it, if we all work together :)

## The problem

## Reference material

- [User Namespaces: 2017 Status Update and Additional Resources](https://integratedcode.us/2017/02/24/user-namespaces-2017-status-update-and-additional-resources/), 02/17
- Phil Estes [Rooting out Root: User namespaces in Docker](https://events.linuxfoundation.org/sites/events/files/slides/User%20Namespaces%20-%20ContainerCon%202015%20-%2016-9-final_0.pdf), 09/2016
- Rami Rosen [Resource management: Linux kernel Namespaces and cgroups](http://www.haifux.org/lectures/299/netLec7.pdf), 05/2013

## Tooling
