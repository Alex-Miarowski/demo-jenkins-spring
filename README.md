# Demo Jenkins Spring 
## Testing the possibilities of Jenkins Pipeline with Spring Boot
Main App has method get() which returns on main endpoint String "Hello world"\
Written test checks if status ok and does the endpoint gives String "Hello world"\
In Jenkinsfile I put 3 stages:
- first is to build app with maven
- second to test with written test
- third is to deploy new app version on heroku

In Jenkins I turned option to automatically start JenkinsPipeline when GitHub gives information about new commit

### _Study Case_:
To work with last option our app cant be hosted on localhost. To get around this we can use ngrok to 'publish' our localhost.