# Couchbase C/C++ Workshop

This page contains details how to use the workshop material.

## Requirements

For the first day each attendee needs to have prepared the following:

* 3 VM-s with CentOS 6
* Static IP addresses
* A ping between the VM-s needs to be possible

For the second workshop days the following is required:

* A C/C++ Development environment which especially includes 'gcc' and 'make'

```
# RHEL6/EPEL
yum install ‚Development Tools'
```

* Qt 5 installed

```
# RHEL6/EPEL
yum install qt
```

* A C/C++ IDE of your choice is installed

```
# RHEL6/EPEL
yum install qt-creator
```

* The IDE needs to be configured to support the Qt libraries

## Agenda

* Day 1

| Time            | Chapter       | Title                                   | Content                                   |
| --------------- | ------------- | --------------------------------------- | ----------------------------------------- |
| 09:00           | 1.1           | Introduction and Core Use Cases         | What is Couchbase Server?                 |
|                 | 1.2           | Couchbase Server Architecture           | Caching Layer, Storage Engine, ...        |
|                 | 1.3           | Couchbase Server as a Distributed System| Intra-Cluster Replication, ...            |
| 10:30           |               | Coffee Break                            |                                           |
|                 | 1.4           | Working with Buckets                    | Create Bucket, add data, ...              |
|                 | 1.5           | Working with the Cluster                | Add/remove Nodes, Server Groups, Rebalance|
| 12:30           |               | Lunch                                   |                                           |
|                 | 1.6           | Security                                | Encrytion, LDAP Integration, Configuration|
|                 | 1.7           | Cross Data Center Replication explained | Setup, Configuration Parameters           |
| 17:00           |               | Q&A and Summary                         |                                           |

## Install the Sample Data

cbdocloader -u couchbase -p couchbase -n 127.0.0.1:8091 -b travel-sample -s 128 travel-sample.zip

