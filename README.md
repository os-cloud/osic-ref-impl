OSIC Reference implementation
=============================

# What is it?

Reference implementation is opinionated way to deploy OpenStack. One of big
qualities of OpenStack is it's flexibility, modularity and amount of underlying
technilogies it can work with. But that also means that it has steep learning
curve as sheer amount of options it allows is overwhelming (some services can
have hundreds of them). We want to ease the entry to OpenStack by providing
what is in our opinion good way to deploy OpenStack. We make sure that it's
possible to be consumed by majority of users because it will be based on
opensource as much as it is reasonable. In short, it's OpenStack authors would
deploy:)

# Design assumptions

RefImpl will be designed to optimally run generic web services/application
workload on a medium scale cloud (20 nodes to start with plans to expand
to 300). Main users of it will be companies that are willing to deploy an
OpenStack private cloud, but have no or minimum OpenStack experience, only
experience as proficient operators. We don't assume any technology they
are using.

Our OpenStack will be:

* production ready - this cloud is meant to serve as production environment
* extensible - extending cloud after initial deployment
* upgradable - it will be as easy as possible to do release upgrades
* easy to deploy - it will require minimal input from operators
* quick to deploy - our goal is to get down to 1min/node on average in scale of 300 nodes
* easy to maintain - we will provide toolset and guidance that will help ops to keep cloud running
* pet friendly - although we suggest move to cloud-native apps, we also recognizes that it can be long process. Our cloud will help to keep non-cloud-native apps running.
