# java-starthere

1. config/DataSourceConfig 
2. controllers/APIsController // api to do data crawling.
3. controllers/LogoutController	// remove in-memory oauth token

## Deploy to Heroku
1. create new app on heroku
2. add-on postgres on heroku and postgres dependency in pom.xml
3. config/DataSourceConfig extracted environment variable into spring-boot beans.
4. Environment variable which was defined in application.properties will be created on heroku variable.
5. include heroku plugin in pom.xml	// for localhost postgres testing
6. change maven goal from 
	* "spring-boot:run" to "clean heroku:deploy -X" // -X to display debug messages.
7. To deploy to remote heroku, execute the application on IDE (intellij Idea or eclipse) locally with usual "run".



