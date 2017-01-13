**GoogleGmailSkill (Mycroft new API)**
===================

For Mycroft with new API (https://home.mycroft.ai)
A skill to use with Mycroft which allow to get emails from your Gmail Inbox.

----------


Installation
-------------------
Is necesary to make this procedure two times

outside mycroft virtual environment for python 2

    sudo pip install google-api-python-client apiclient oauth2client httplib2



Now enter inside mycroft virtual environment

Inside mycroft virtual environment

    workon mycroft

    pip install google-api-python-client apiclient oauth2client httplib2


Now go to Mycroft skills folder

    cd  $HOME/.mycroft/skills

    git clone  https://github.com/jcasoft/GoogleGmailSkill.git

<i class="icon-cog"></i>Add 'GoogleGmailSkill' section in your Mycroft configuration file on:

    $HOME/.mycroft/mycroft.conf

  	"GoogleGmailSkill": {	
	    "loginEnabled": true,
	    "maxResults": 10,
	    "time_format": 12	# 12 for AM/PM and 24 for 24 hours time format
	}



Authorize Google GMail Skill in distro with local web browser, wait web browse open and select "Allow"

    From your command line go to mycroft skills folder

    cd  $HOME/.mycroft/skills

    python GoogleGmailSkill

	
Authorize Google GMail Skill in distro without local web browser

    From your command line go to mycroft skills folder

    cd  $HOME/.mycroft/skills

    python GoogleGmailSkill --noauth_local_webserver

Open the generated link in computer with browser and wait the verification code and paste

     Enter verification code: 4/oxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx   



Restart Skills

    ./start.sh skills

----------


Features
--------------------

Currently this skill can do the following things to get information from your Gmail Inbox, un-read e-mails (with some variation):

- Check my gmail
- Get my last gmail
- Get my last gmail complete 
- Get my last gmail detailed
- Get my last gmail with detail 
- Get my last gmail with body   
- Get my last 5 gmail
- Get my last 6 gmail complete 
- Get my last 7 gmail detailed
- Get my last 8 gmail with detail 
- Get my last 9 gmail with body
- Get my gmail


> **Note:**

> - You can toggle key word with:
> - The words: complete, detailed, with detail, with body; offer the same results




**Enjoy !**
--------