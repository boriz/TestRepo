# TestRepo

Configure git
Configure editor in the global config file: 
git config --global core.editor "'C:/Program Files (x86)/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"

Install Arcanist: https://secure.phabricator.com/book/phabricator/article/arcanist/
php and arcanist\bin should be in the path

Create .arcconfig file:
{
  "phabricator.uri" : "http://dmc-phab.cloudapp.net/"
}

Configure text editor:
arc set-config editor "\"C:\Program Files (x86)\Notepad++\notepad++.exe\" -multiInst -nosession"

Install certificates:
arc install-certificate
It will ask you to navigate to: http://dmc-phab.cloudapp.net/conduit/login/
At this URL you should see an API token, copy/paste it.

Review request
arc diff
Eneter required fields (reviewers/subscibers has to match user names)
