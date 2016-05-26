# MSTC CRM with OTSM

**Multiple Sclerosis Therapy Centre Client and Resource Management with Oxygen Therapy Session Management**

An open source, Ruby on Rails project to provide Multiple Sclerosis Therapy Centres an integrated tool to manage clients, resources and oxygen therapy sessions.  

Initially created for the MS Therapy Centre Lothian http://www.mstc-lothian.org.uk/

The software is intended to be run onsite on a dedicated linux based server.

Pull requests and bug reports are always welcome!

### Contents
- [Installation](#installation)

## Initial Developmet

Text files have been created (found under ./doc/) giving a very basic listing of features that are required or desired.  These documents should provide a general idea of the controlers and data fields which need to be created.

## Installation for Development

### Requirements

Before you get started, the following needs to be installed:

  * **Ruby**. Version 2.2.4 (Windows) or 2.3.1 (Linux)
  * [**RubyGems**](http://rubygems.org/)
  * **Bundler**: `gem install bundler`
  * [**Git**](http://help.github.com/git-installation-redirect)

Grab the code:

```
git clone git://github.com/kmclellan/mstc.git
```

Install the dependancies:

```
cd mstc
bundle install
```

Initiate your development database:

```
bundle exec rake db:create
bundle exec rake db:migrate
```

(Currently do not have a schema to load.)

To view the application run a Rack webserver.  In production this will be Phusion Passenger (simple and reliable deployment).  For development I am currently using Thin.

```
bundle exec thin start
```

http://localhost:3000


## Contributing

Please see CONTRIBUTING.md for more detail.

 - Fork the repository using Github.
 - Checkout a named feature branch created from the development branch.
 - Write tests using rspec.
 - Complete modifications or corrections.
 - Run the tests, ensuring they all pass. (See TESTING.md)
 - Contact lead developer, describe work done, submit a Pull Request to the development branch using Github.

If you have direct access to the repository then develop in a branch before merging to master.  DO NOT DEVELOP IN THE MASTER BRANCH.

## License / Copyright

The software is released under an open source MIT license (please see copyright file).