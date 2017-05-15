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

Organisers
``````````

Slug: ``pyconuk-organisers``

A standard slack team with no changes to settings.

Admins are:

* Charlie
* George
* Kristian
* Peter


Attendees
`````````

Thanks to `Baptiste Mispelon <https://twitter.com/bmispelon>`_ for his help with getting this slack set up.

Slug: ``pyconuk-2016``

Admins are:

* Charlie
* Cory
* George
* Kristian
* Peter

Settings
~~~~~~~~

* Team Signup Mode: **Invitation only**
* Default Channels: **#announcements, #social**
* Username Guidelines: **Default**
* Name Display: **Display usernames**
* Require @ for mentions: **No**
* Do Not Disturb: **8PM -> 9AM**
* Hide your team URL from external sites' logs: **Yes**
* Calls: **No**
* Team Icon: **Yellow Python (/media/img/yellow.png)**
* Team Name & URL: **PyCon UK 2016 & pyconuk-2016**


Permissions
~~~~~~~~~~~

* Messaging:

  * *People who can use @channel and @here:* **Team Owners only**
  * *Show a warning when using @channel or @everyone:* **Always**
  * *People who can post to #general:* **Everyone**
  * *People who can use @everyone:* **Team Owners only**

* Invitations: **Don't allow everyone**
* Channel Management:

  * *People who can create private channels:* **Team Owners only**
  * *People who can create channels:* **Team Owners only**
  * *People who can archive channels:* **Team Owners only**
  * *People who can remove team members from private channels:* **Team Owners only**
  * *People who can remove team members from channels:* **Team Owners only**

* Message Editing & Deletion:

  * *Allow editing:* **Never**
  * *People who can delete messages:* **Team Owner and Admins only**

* Stats: **Team Owner and Admins only**
* Custom Emoji & Loading Messages:

  * *People who can manage custom emoji:* **Team Owner and Admins only**
  * *People who can manage custom loading messages:* **Team Owner and Admins only**

* Slackbot Responses: **Enabled**

  * *People who can add Slackbot responses for your team:* **Team Owner and Admins only**

* Public File Sharing: **Yes**
* Gateways:

  * *XMPP (SSL only):* **Yes**
  * *IRC (SSL only):* **Yes**
  * *IRC (no SSL):* **No**


Invitations
~~~~~~~~~~~
New members can be invited by Owners or Admins `here <https://pyconuk-2016.slack.com/admin/invites>`_.

Slack places limits on invitations when the accepted:sent ratio is low. See `here for more details <https://get.slack.help/hc/en-us/articles/201330256#invitation_limits>`_.
