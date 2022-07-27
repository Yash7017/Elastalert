# Elastalert
Setting up Elastalert to raise alert for patterns and keywords. While we want to setup up alerts for increasing a particular patterns or keywords in the file. then we use the elastalert and postfix as SMTP server. 

**To be noted** : Here we are raising alerts and sending them to Email only. i will attach more links to raise the alert for other platforms also like jira or slack. if you need any of them please visit them. 

This was the best configuration, I came through to install Elastalert. But there was an issue while installing it for me. Few configuration was not compatible with python. i was supposed to add more packages to work on that. 

###### In the same tutorial, I used python3 and pip3 everywhere on the place of python and pip respectively. You can follow through with the video. apart from that i will add on the code that i executed to make it work. you can try with python, if that doesn't work with you also and give errors to download different packages everytime, even you install that still giving same error then use pip3 and python3 to make it work.



https://www.youtube.com/watch?v=vhRxUrg2OxM

https://github.com/justmeandopensource/elk/blob/master/docs/elastic-kibana-filebeat-elastalert-notes.md


## Start Elastalert

if you are using python3 and pip3 then you will have to start Elastalert using. **you will have to go inside the elasalert folder then run it. where your config.yaml file exist otherwise it will raise error.**

```
python3 -m elastalert.elastalert --verbose --config config.yaml
```

if you are using python and pip then you can use python instead of python3. 

I have updated a few more things in my code, thats why i am using config.yaml. I have made multiple yaml file rules to raise alert and put them in a new folder. Inside config.yaml file, i gave path to that folder.

I have attached code of my config.yaml and frequency_rules in the code section. check them out if you are already following my ELK setup. You will have to give Elastic username and password also to let elastalert have access of your logs.   

**Go through more repositories for example_frequency.yaml setup. 

https://github.com/Yelp/elastalert/blob/master/example_rules/example_frequency.yaml
https://github.com/Yelp/elastalert/tree/master/example_rules
