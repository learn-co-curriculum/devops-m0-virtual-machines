# Virtual Machines

## Learning Goals

- Understand the concept of virtualization
- Learn how virtual machines operate
- Understand the benefits and limitations of virtual machines

## Introduction

A **virtual machine**, as the name implies, is virtual; in other words, it's not a physical machine. Virtual machines are created using a process known as **virtualization**, which simply creates a virtual version of something, in this case, a full-fledged computer system. Virtual machines are utilized throughout the industry for all sorts of applications, and we will be making extensive use of them in this course.

Virtual machines have been around since the 1960s, thanks largely to *IBM's* development of logical partitions, which allowed a single computer mainframe to run multiple instances of operating systems simultaneously. 

That being said, it wasn't until the late 1990s that virtualization technology seriously took off, when hardware-assisted virtualization starting become ubiquitous. These advancements led to the widespread adoption of virtualization in the enterprise sector and the growth of the cloud computing industry.

In the modern day, virtualization is an essential component of computing, with all major computing platforms supporting it in some form.

## What are VMs used for?

The ability to isolate an entire system gives users a lot of advantages, including:

- **Sandboxing:** You can run anything you want inside a virtual machine with little risk since due to its contained nature. This allows for secure and reliable testing without impacting the rest of the system.
- **Replication:** Virtual machines can be backed up and restored with ease, allowing users to replicate systems very easily. If a system fails or becomes compromised, rolling back is an easy option.
- **Running incompatible software:** You can run other operating systems in virtual machines, allowing you to make use of software available only in a specific OS.
- **Compartmentalization**: Virtual machines allow you to split up a host system into multiple guest systems, allowing for clean separation between them.

That being said, it's not all rainbows and sunshine with virtual machines; they have some disadvantages as well:

- **Performance**: Virtual machines typically do not perform as well as their host computer due to the overhead that comes with virtualization. The difference depends on the virtualization technologies being used.
- **Complexity**: Setting up and managing virtual machines can be complex and time-consuming, and if you have to allocate resources ahead-of-time, adds a non-negligible amount of mental overhead
- **Storage**: While a smaller issue, virtual machines can end up consuming a significant amount of storage space depending on the environments installed on them.

This makes virtual machines particularly useful for **cloud computing**. Cloud vendors typically offer resources online on a pay-as-you-go model; virtual machines vastly facilitate this by allowing vendors to separate a machine based off individual client demands. This means vendors can quickly and easily scale their computing resources up or down as needed, without the need to purchase and maintain physical hardware.

![virtualization](https://curriculum-content.s3.amazonaws.com/6685/devops-m0-virtual-machines/virtualization.png)

## Setting up a virtual machine

In our case, since our host computers are most likely *not* running *Linux*, we will be making use of virtual machines to gain access to a fully-featured server *Linux* distribution. In the case you are actually running *Linux*, you should still use a virtual machine to keep all the services contained instead of polluting your personal computer with services only needed for this course.

If you are using *Windows*, *Mac* (*Intel*), or *Linux* desktop, please follow the **64-bit setup** installation guide.

If you are using an *Apple*-silicon *Mac* (M1, M2, etc.), please follow the **Apple-Silicon** installation guide.

Mac users can verify what type of Mac they have by clicking the Apple logo and selecting `About This Mac`. If it doesn't say `Apple` under chip, then you have an Intel Mac.

## Conclusion

Virtualization is both ubiquitious and crucial to understand in the modern computing world. This will become clear once you familiarize yourself with your own virtual machine, and later take a look at many of the services offered by leading cloud providers (*AWS*, *Azure*, *Google Cloud*).
