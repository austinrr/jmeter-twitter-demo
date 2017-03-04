# JMeter Api Test Demo

### Gettin started:
- Download repo & run the following:

Mac
```sh
.../jmeter-twitter-demo/apache-jmeter-3.1/bin/jemter.sh
```
**OR**

Windows
```cmd
...\jmeter-twitter-demo\apache-jmeter-3.1\bin\jemter.bat
```

- Open the project **twitter_api.jmx**


### Run the Test
```sh
1. (optional) press the blue + icon to expanpand the tree so you can see all the samplers and assertions
2. press the green play button to run the test.
3. click on the 'view results tree' listener to examine the results.
```

### Results!
![alt tag](https://github.com/austinrr/jmeter-twitter-demo/blob/master/screen1.png)


### Notes
This API test is admittedly fairly simple, but it does execute some positive and negative cases.  The real challange here was getting OAuth to work.  Currently this example used a bearer key I generted using a fresh twitter account connected to dev.twitter.com application portal.  Initailly I tried using OAuth 1.1a but I ran into some problems with the JMeter plugin and the signpost JAR, so Oauth 2.0 turned out to be much simpler.  I would like to also point out that JMeter can be run headless and generate a variely of reports.  It's also possible to run distributed.  The main drawback is that the open source natures results in some instability and a reliance on plugins for some functionality.

--P.S. I will be invalidating my twitter bearer token in a few days since this is public--
