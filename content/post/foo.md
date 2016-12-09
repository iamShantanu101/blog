+++
title = "Docker - The Supernovae in the Tech Galaxy"
slug = "post-title"
tags = [
  "Docker",
  "Containerization",
]
comments = true
share = true
image = ""
menu = ""
date = "2016-12-08T22:02:29+05:30"
draft = false
author = "Shantanu"

```bash
echo "hello world !!"
```

+++

The basic tenant of the Type 1a supernova paradigm is that these explosions happen when a group of exhilaratingly passionate guys gets close to a tipping point - A stable version (or even alpha/beta). They then open source the store of potentially great stuffs to a large open source community. The resulting explosion spreads like a fire, leaving an ever exapnding cloud of features dominated by the creators and open source community. So far, so good.

Ah, without much ado, lets break the surprise! This was none other than; Docker - The Supernovae in the Tech Galaxy.

![Docker](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_(container_engine)_logo.png)

Confused? Since when did a giant Blue Whale carrying some blocks is a Supernovae? Lets see how this goes.

**What is Docker?**

As the official overview says :

PACKAGE YOUR APPLICATION INTO A STANDARDIZED UNIT FOR SOFTWARE DEVELOPMENT

Docker containers wrap a piece of software in a complete filesystem that contains everything needed to run: code, runtime, system tools, system libraries – anything that can be installed on a server. This guarantees that the software will always run the same, regardless of its environment.

**Now what the heck are Docker containers anyways? Or just Containers? And why do I need them?**



Containers are a solution to the problem of how to get software to run reliably when moved from one computing environment to another. This could be from a developer's laptop to a test environment, from a staging environment into production and perhaps from a physical machine in a data center to a virtual machine in a private or public cloud.

Problems arise when the supporting software environment is not identical, says Solomon Hykes, the creator of Docker, "You're going to test using Python 2.7, and then it's going to run on Python 3 in production and something weird will happen. Or you'll rely on the behavior of a certain version of an SSL library and another one will be installed. You'll run your tests on Debian and production is on Red Hat and all sorts of weird things happen."

And it's not just different software that can make a difference, he added, "The network topology might be different, or the security policies and storage might be different but the software has to run on it."

**How do containers try to solve this problem?**

Put simply, a container consists of an entire runtime environment: an application, plus all its dependencies, libraries and other binaries, and configuration files needed to run it, bundled into one package. By containerizing the application platform and its dependencies, differences in OS distributions and underlying infrastructure are abstracted away.

**Sounds like Virtualization, right? Whats the difference then?**

In virtualization technology, the package that can be passed around is a virtual machine. This means it includes an entire operating system as well as the applciation. A physical server running three VMs would have a hypervisor and three OSs running on top of it.

On the contrary, a server running the containerized applications as with Docker runs a single OS, and each container shares the OS kernel with the other containers.Shared parts of the operating system are read only, while each container has its own mount (i.e., a way to access the container) for writing. That means the containers are much more lightweight and use far fewer resources than virtual machines.

**What difference will it make in practical scenario?**

A container may be only tens of megabytes in size, whereas a virtual machine with its own entire operating system may be several gigabytes in size.

Because of this, a single server can host far more containers than virtual machines. Virtual machines may take several minutes to boot up their operating systems and begin running the applications they host, containerized applications can be started almost instantly.

**If containers share an operating system, how secure can this be?**

The general consensus, as of now, is that containers are not as secure as virtual machines. The reason is, if there's a vulnerability in the kernel, it could provide a way in to the containers that are sharing it (although SELinux can help.) That's also true with a hypervisor, but since a hypervisor provides far less functionality than a typical Linux kernel (which typically implements file systems, networking, application process controls and so on) it presents a much smaller attack surface.

To summarize, containers cannot generally provide the same level of isolation as hardware virtualization.

**Now what's the difference between Docker and containers?**

Docker has become synonymous with container technology because it has been the most successful at popularizing it. But container technology is not new: It has been built in to Linux in the form of LXC for almost 10 years, and similar operating system level virtualization has also been offered by FreeBSD jails, AIX Workload Partitions and Solaris Containers.

And today Docker is not the only game in town for Linux. One notable alternative is rkt, a command line tool for running app containers produced by CoreOS. Rkt is able to handle Docker containers as well as ones that comply with its App Container Image specification.

What's next? Stay tuned for the next post to dive deeper! Thanks!


