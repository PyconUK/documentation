Set up the conference Slack
===========================

Organisers
**********

URL: `pyconuk-organisers.slack.com <pyconuk-organisers.slack.com>`_

A standard Slack team with no changes to the default settings.

You can see a full list of admins in `the Slack admin panel
<https://pyconuk-organisers.slack.com/account/workspace-settings#admins>`_.
At time of writing (11 September 2018), the admins were:

*  Charlie
*  Daniele
*  George
*  Kristian
*  Owen
*  Peter

Attendees
*********

This is usually created a week or so before the conference starts.

Thanks to `Baptiste Mispelon <https://twitter.com/bmispelon>`_ for his help with getting this Slack set up in 2016.

The slug is ``pycon-{year}``, e.g. ``pycon-2016``.

Admins are usually whoever's on the organising committee for that year.

Settings
--------

* Team Signup Mode: **Invitation only**
* Default Channels: **#announcements, #social**
* Username Guidelines: **Default**
* Name Display: **Display usernames**
* Require @ for mentions: **No**
* Do Not Disturb: **8PM -> 9AM**
* Hide your team URL from external sites' logs: **Yes**
* Calls: **No**
* Team Icon: **Yellow Python (slack_avatar.png)**
* Team Name & URL: **PyCon UK 2016 & pyconuk-2016**

.. image:: /_static/slack_avatar.png

Permissions
-----------

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
-----------

New members can be invited by Owners or Admins at ``https://pyconuk-{year}.slack.com/admin/invites``.

Slack places limits on invitations when the accepted:sent ratio is low. See `here for more details <https://get.slack.help/hc/en-us/articles/201330256#invitation_limits>`_.


Channels
--------

At time of writing (13 September 2018, pyconuk-2018), we had the following
public channels:

*  announcements (admins only)
*  av
*  djangogirls
*  feedback
*  general_chat
*  helpdesk
*  introductions
*  recruitment
*  social
*  talks
*  undefined

And private channels:

*  chairs
*  contributors
*  djangogirlscoaches
*  helpdesk-helpers
*  sponsors

The following channels are auto-joined when somebody signs up (configured in
Settings > Default Channels):

*  announcements
*  helpdesk
*  introductions
*  social
*  undefined

.. note:: We have the metadata in Ironcage to detect if somebody is a
          contributor, sponsor, etc.  It would be a nice future enhancement
          to set up a way to auto-join people to the appropriate extra
          channels.
