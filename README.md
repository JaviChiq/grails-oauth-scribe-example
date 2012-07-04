# grails-oauth-scribe-example

Example Grails project showing integration with multiple OAuth providers using scribe-java.
Currently supports Google+, Facebook, Twiiter, GitHub and LinkedIn.
It uses underneath [scribe-java](https://github.com/fernandezpablo85/scribe-java) library.

# Installation

Clone repository and try to start grails:
```grails run-app```

If succeed, you have to register your application to various OAuth providers, see table below:

<table>
<tr><th>Provider</th><th>Where to register application</th></tr>
<tr><td>Google+</td><td>https://code.google.com/apis/console</td></tr>
<tr><td>Facebook</td><td>https://developers.facebook.com/apps</td></tr>
<tr><td>Twitter</td><td>https://dev.twitter.com/apps/new</td></tr><tr><td>GitHub</td><td>https://github.com/settings/applications/new</td></tr>
<tr><td>Linkedin</td><td>https://www.linkedin.com/secure/developer?newapp=</td></tr>
</table>

Then, rename ```oauth.properties.template``` from grails-app/conf to ```oauth.properties``` and copy the API and secret keys to corresponding property of the file.
Example of Google below:

![google](http://i.imgur.com/zhfBe.png)

You should now be able to login with your social accounts. Beware of callback URLs - not all providers support application hosted on localhost :( But deploying on [cloudfoundry](http://grails.org/plugin/cloud-foundry/) should help.

Enjoy!

