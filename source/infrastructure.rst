Infrastructure
==============

The PyCon UK infrastructure is comprised of the following services:

**Website**

* GitHub for code
* GitHub for hosting
* Travis-CI for code testing
* DNSimple for DNS
* 123-reg is the ``pyconuk.org`` domain registrar


**Ticketing**

* ti.to


**Organisation**

* GitHub for Issues
* GitHub for docs code
* ReadTheDocs for docs hosting


**SMS App**

* GitHub for code
* Twilio for SMS delivery


**Voting App**

* Heroku for hosting
* GitHub for code
* Opbeat for Error tracking


**Chat**

* Slack for organisers
* Slack for attendees


This boils down to the following Vendors:

* 123-reg
* DNSimple
* GitHub
* Heroku
* Opbeat
* ReadTheDocs
* Slack
* ti.to
* Travis-CI
* Twilio


Pricing
-------

Ti.to
`````
Based on their `pricing page <https://ti.to/pricing>`_ and using the dummy values of 300 tickets at £200p/ticket (note: not actual values) we would be looking at paying between £3176.46 and £3600.

GitHub
``````
Free. We should have no need for private repositories as things currently stand.

Travis-CI
`````````
Free. We currently have no private repositories and can stay on the community offering.

ReadTheDocs
```````````
Free. We're currently using their free offering which I don't expect to change.

Heroku & Opbeat
```````````````
We have yet to discuss whether the Voting app will be needed this year but it's currently running on free versions of both Heroku & Opbeat.

123-reg & Twilio
````````````````
Waiting on information.

DNSimple
````````
$50 per year for a single user account, limited to 5 domains. We should only need the one domain.


DNS
---
Each year's website has a subdomain under ``pyconuk.org`` (eg 2016.pyconuk.org) with a matching repo in `our GitHub organisation <https://github.com/pyconuk>`_.

DNSimple is configured with a CNAME for each year hosted on GitHub Pages (2015 onwards). URL records have been set up to redirect ``pyconuk.org`` and ``www.pyconuk.org`` to the appropriate year subdomain.

Years prior to 2015 have A records pointing them to a server kindly hosted by Zeth.


Passwords
---------
Account passwords are currently in a 1Password vault that only George has access to. This needs to be improved.


Website Deployment
------------------
The website can be built and deployed locally by running ``make deploy``. However this is not ideal when using a Pull Request workflow since it requires someone to have a working environment and thus TravisCI has been set up to deploy changes made to master.

For more details on this see `the website readme <https://github.com/PyconUK/2016.pyconuk.org#deployment>`_.


Slack
-----

See :doc:`the Slack howto guide <howto/setup-slack>`.

GitHub Permissions
------------------

Owners are:

* Charlie
* Cory
* George
* Kristian
* Owen
* Peter

Two main teams:

* Core: Basically everyone
* pydata: PyData related folk


Giving Push Access
``````````````````
Most of our repos are public so forking and PRing are simple, however on heavier usage repos (main website, ironcage, etc) it can be easier to just allow write access.

Make sure the repo in question is added to the core team `here <https://github.com/orgs/PyconUK/teams/core/repositories>`_ and has ``Write`` permissions.
