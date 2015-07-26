#Baker Street

Baker Street is a service discovery and routing system designed for microservice architectures.

Baker Street simplifies scaling, testing, and upgrading microservices by:

* focusing on high availability and eventual consistency of the overall system
* enabling canary testing for staged testing and deployment of service upgrades
* supporting language, framework, and tooling independence for developers

Baker Street consists of three components:

* Sherlock - a routing system with local instances corresponding to each instance of your application to determine where connections from that instance should go
* Watson - a health checker with local instances corresponding to each instance of your application
* Datawire Directory - a global registration service recording server availability that receives availability information from each Watson instance and pushes changes in availability to local Sherlock instances as needed.

##Baker Street System Requirements

Baker Street works on any flavor of Enterprise Linux 7 or on Ubuntu 14.04 LTS. It has no other requirements, but since it must be co-located with your service, your service must also run on one of these platforms if you wish to use it with Baker Street.

##Installing Baker Street

We expect it to take approximately 15 minutes to install a working local development environment with all three components.

Directions for installing Baker Street locally can be found [here](http://bakerstreet.io/docs/quickstart.html#setup).

##Next Steps

Additional information about Baker Street's design and architecture can be found [here](http://bakerstreet.io/docs/architecture.html).

Baker Street components all support a variety of options available via configuration files. For example, each component supports a range of logging levels that can be independently toggled within these configuration files. Information on how to configure each component can be found [here](http://bakerstreet.io/docs/reference.html).

##Additional Information

For additional information, visit the Baker Street website at [http://www.bakerstreet.io](http://www.bakerstreet.io).

Please post any questions about Baker Street on [Stack Overflow](http://www.stackoverflow.com) using the tag bakerstreet.
