# jiraslackbot

A slackbot(https://slack.com/intl/en-gb/help/articles/202026038-An-introduction-to-Slackbot) plugin will require a JIRA API to request the information with the reference about a ticket when mentioned in the slack channel.

## How to Install

1. The slackbot can be installed with the command pip3 install slackbot or it can be cloned from https://github.com/lins05/slackbot

2. `pip install slackbotjira`

3. In slackbot_settings.py:
  * 'slackbotjira' should be added to the PLUGINS list
  * `import os` needs to be done in order to use environment variables for JIRA username/password
  * Python variables should be configured in slackbot_settings.py
    * JIRA_URL = '{JIRA URL}'
    * JIRA_AUTH = (os.environ['JIRA_USER'], os.environ['JIRA_PASS'])
    * JIRA_PROJECTS = ['SPT']  # JIRA Project Keys
    
4. Configure Environment Variables for Authorization
  * JIRA_USER
  * JIRA_PASS

