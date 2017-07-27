# Non-privileged containers FTW!

Did you know that running containers with user `root` is not only a bad practice but really is a security risk?
You might not care when launching a single container on your laptop, but in the context of container orchestrators such as Kubernetes, this is a real problem. This site tries to explain the issue, collects data and reference material and ultimately provide you with tooling to change the status quo. We can do it, if we all work together :)

## The problem

TBD.

## Reference material

### Official docs

- [Docker security](https://docs.docker.com/engine/security/security/#linux-kernel-capabilities)
- CoreOS [rkt Capabilities Isolators Guide](https://coreos.com/rkt/docs/latest/capabilities-guide.html)
- OpenShift [Managing Security Context Constraints](https://docs.openshift.org/latest/admin_guide/manage_scc.html)

### Related activities and discussions

- [contained.af](https://contained.af/) by Jess Frazelle
- [containerhardening.org](https://containerhardening.org/) by Jess Frazelle
- [rootlesscontaine.rs](https://rootlesscontaine.rs/) by Aleksa Sarai
- [Getting Towards Real Sandbox Containers](https://blog.jessfraz.com/post/getting-towards-real-sandbox-containers/) by Jess Frazelle
- [Docker and CIS Benchmark](http://blog.aquasec.com/docker-1.11-and-cis-benchmark-whats-new-in-security) 
- [CIS Benchmark for Kubernetes 1.6](http://blog.aquasec.com/cis-benchmark-for-kubernetes-security)
- The ThoughtWorks Technology Radar on [container security scanning](https://www.thoughtworks.com/radar/techniques/container-security-scanning)
- [Privileged Docker Containers](http://obrown.io/2016/02/15/privileged-containers.html)
- SO question on [Privileged containers and capabilities](https://stackoverflow.com/questions/36425230/privileged-containers-and-capabilities)

### Background

- [User Namespaces: 2017 Status Update and Additional Resources](https://integratedcode.us/2017/02/24/user-namespaces-2017-status-update-and-additional-resources/), 02/17
- Phil Estes [Rooting out Root: User namespaces in Docker](https://events.linuxfoundation.org/sites/events/files/slides/User%20Namespaces%20-%20ContainerCon%202015%20-%2016-9-final_0.pdf), 09/2016
- Rami Rosen [Resource management: Linux kernel Namespaces and cgroups](http://www.haifux.org/lectures/299/netLec7.pdf), 05/2013
- Michael Cherny [Docker Security Features, Part 3: User Namespace](http://blog.aquasec.com/docker-1.10-user-namespace), 03/2016

## Tooling

- [Quay Security Scanner](https://coreos.com/quay-enterprise/docs/latest/security-scanning.html)
- [Docker Security Scanning](https://docs.docker.com/docker-cloud/builds/image-scan/)
- [Aqua Security Scanning and Runtime protection](http://blog.aquasec.com/docker-security-best-practices) 

