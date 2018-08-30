# MultiRequests

A system for fast and robust anonymised parallel requests with information sharing over a pool of unreliable proxies to a potentially unfriendly peer.
Although not suggested use case, potentially a tool for carrying out spamming, scraping, and captcha avoidance without a botnet or paid proxies.
Provides additional features such as commandline printout of the proxy pool and the success rate over time.

![Program Architecture Diagram](https://github.com/raskellr/test/blob/master/images/Diagram.jpg)

## Use Cases
Unreliable proxies
Circumvent blacklisting/throttling of ip addresses, including paid and unpaid proxies

### Prerequisites

(Optional) Install [hipsterplot](https://github.com/imh/hipsterplot)

Python3

### How to use
The user must implement:
The data classes for for the superclass Data, which must implement the following methods:
```
__init__, __str__, next
```
As __str__ will serve as a unique identifier, 

The batch_handler instance which initiates and runs the MultiBatchHandler session, and pipes around data. 
The call function to a particular webservice, which returns signals (success, score, completed, switch) to the batch handler for scoring proxies and rotating data and proxies. 
The right settings for the various handlers, such as optimal number of proxies in pool, number of batch_handler processes, amount of staggering to initial batches to avoid network spike detection, timeout parameters for the http request tests and the deployment environment calls, thresholds for proxy blacklisting and proxy and data switching. 



```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
