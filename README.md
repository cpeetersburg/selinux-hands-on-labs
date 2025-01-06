# Introduction

During my career as a consultant at a Red Hat Premier Partner, it became very clear to me that very few people actually understand SELinux, let alone implement it in their environments. Many companies I have worked with simply turn it off as a matter of course. I have even seen commercial software distributed for Enterprise Linux distributions which lists disabling SELinux as a mandatory installation step. As a result I felt it prudent that I get to grips with this technology both for my own understanding, and to help others.

With the advent of the GDPR simply turning off SELinux is no longer acceptable as a solution. Whilst this project does not intend to get into any debate on the meaning or implementation of the GDPR, it is based on the premise that in the event of an attack on a system (whether that attack was successful or not), it would have been better to have taken advantage of this additonal security layer than to have simply turned it off because it was deemed too complex or difficult to get working.

# Scope

At this stage, this project does not aim to provide a comprehensive coverage of SELinux - it is a huge and powerful security layer and there are many excellent references texts on it. I have always learned better by doing than by learning through theory, so I decided to come up with a set of labs where you can safely learn some of the more common SELinux fundamentals and hopefully demystify it.

As such the scope of this project is a very common scenario that I have come up against many times in my career:

* The application to be secured is not SELinux aware and has no specific coding to work with or alongside SELinux
* The hosting machine is running Red Hat Enterprise Linux or a derivative (e.g. Rocky or CentOS Stream)
* (new for 2025) All labs have been tested on Fedora 41 Server also
* The host machine has SELinux enabled and in `enforcing` mode
* The host machine is using the `targeted` policy

MLS (Multi-Level Security) is beyond the scope of this project at this stage but may be added if there is a requirement for it.

# Getting started

I have endeavoured to provide all the information you need to get started and run these labs, and more information can be found in Lab 1 which I recommend you proceed to straight away. I do recommend working through these labs on a VM set aside for this purpose as although the labs are designed to be self contained and not affect the other part of the host system, any tinkering or testing things outside the bounds of the lab (which is highly recommended if it helps you learn more!) could have an undesirable effect on the system.

# Credits

There have been many many sources that have helped me put this project together and I have tried to include them in the comments section of each file where relevant. Special mention is deserved to:

* Red Hat Enterprise Linux documentation: https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/9/html/using_selinux/index
* Gentoo Linux for their excellent SELinux tutorials - found at: https://wiki.gentoo.org/wiki/SELinux/Tutorials
* Sven Vermeulen for his SELinux Cookbook

