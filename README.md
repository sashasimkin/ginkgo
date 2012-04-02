# Ginkgo v0.5.0dev

Lightweight service framework on top of gevent, implementing the "service model" -- services all the way down.

Please note that this version is major rewrite since 0.3.1, hence
skipping 0.4.0. Take a look at UPGRADING and some of the documentation
might be out of date during transition.

## Features
* Service model -- Break your app down into services and sub-services.
  Modules, if you will, that can start, stop, and reload. Every service
  manages its own pool of greenlets.
* Configuration -- Built-in, reloadable configuration based on Python
  files. Access configuration settings relative to services.
* Runner -- Command-line tool to manage your service that can daemonize,
  chroot, drop privs, and set up or override configuration.

## Demo
A talk was given at PyCon 2012 called "Throwing Together Distributed
Services with gevent" that used Ginkgo to build a number of simple
services combined to make a more complex distributed service.

* [PyCon 2012 Video](http://pyvideo.org/video/642/throwing-together-distributed-services-with-geven)
* [PyCon 2012 Slides](http://dl.dropbox.com/u/2096290/GinkgoPyCon.pdf)
* [Source code used in talk](https://github.com/progrium/ginkgotutorial)

## Mailing List

Pretty active discussion on this early microframework. Join it or just
read what's being planned:

* [Ginkgo-dev Google Group](http://groups.google.com/group/ginkgo-dev)

## Contributing

Feel free to poke around the issues in the main repository and see if you can tackle any. From there you should:

* Fork if you haven't
* Create a branch for the feature / issue
* Write code+tests
* Pass tests (using nose)
* Squash branch commits using [merge and reset](http://j.mp/vHLUoa)
* Send pull request

We highly recommend using branches for all features / issues and then squashing it into a single commit in your master before issuing a pull request. It's actually quite easy using [merge and reset](http://j.mp/vHLUoa). This helps keep features and issues consolidated, but also makes pull requests easier to read, which increases the speed and likelihood of being accepted.

We're aiming for at least 90% test coverage. If you have the `coverage` Python package installed, you can run `python setup.py coverage` to get a coverage report of modules within gservice.

## Contributors

 * [Jeff Lindsay](jeff.lindsay@twilio.com)
 * [Sean McQuillan](sean@twilio.com)
 * [Alan Shreve](ashreve@twilio.com)
 * [Chad Selph](chad@twilio.com)
 * [Ryan Larrabure](ryan@twilio.com)
 * [Marc Abramowitz](marc@marc-abramowitz.com)
 * [David Wilemski](david@davidwilemski.com)

## License

MIT

