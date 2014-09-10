social-scoreboard
=================

This application will be used to share the score of a basketball game between several people. 

There will be a person attending the match and she will go updating the result for other people who are not there.

To install:

```bash
npm install
```

server
======

To test with Cucumber:

```bash
grunt
```

client
======

To install:

```bash
bower install
```

To start Web server

```bash
grunt client-dev-run
```

deploy to OpenShift
===================

To merge ([see this](http://stackoverflow.com/questions/12657168/can-i-use-my-existing-git-repo-with-openshift)):

```bash
git clone <GitHub-repo-url>
git remote add openshift -f <openshift-git-repo-url>
git merge openshift/master -s recursive -X ours
```

To push changes:

```bash
git push openshift HEAD
```
