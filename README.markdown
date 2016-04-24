## Getting Started

This project makes it dead-simple to deploy Storm clusters on AWS. See [the wiki](https://github.com/nathanmarz/storm-deploy/wiki) for instructions on using this deploy.

## Acknowledgements

YourKit is kindly supporting open source projects with its full-featured Java Profiler. YourKit, LLC is the creator of innovative and intelligent tools for profiling Java and .NET applications. Take a look at YourKit's leading software products: [YourKit Java Profiler](http://www.yourkit.com/java/profiler/index.jsp) and [YourKit .NET Profiler](http://www.yourkit.com/.net/profiler/index.jsp).

## Custom Updates

* Updated default branch to `free-tier`
* Updated conf/clusters.yaml to work with AWS free tier
 * 2 supervisor nodes => 1 supervisor node
 * set all instance types to `t1.micro` (`t2.micro` not supported by [`jclouds`](https://issues.apache.org/jira/browse/JCLOUDS-621))
 * set all images to ubuntu-trusty-14.04-amd64-server-20160114.5 (`ami-b2e3c6d8`)
