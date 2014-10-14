Get started with e2esqldb
-----------------------------------
This is a template for Bluemix Java Web database application development.

The sample is a simple todo list where users can add, modify, and delete individual todo items, while those items persist to the backend database. In the sample is a clear demonstration of how to use JPA or JDBC to access the database service that binds to the application.

1. [Install the cf command-line tool](https://www.stage1.ng.bluemix.net/docs/#starters/BuildingWeb.html#install_cf).
2. [Download the starter package](https://ace.stage1.ng.bluemix.net:443/rest/../rest/apps/2c299d3b-f02e-41f4-a9b7-29b53b26e1b0/starter-download).
3. Extract the package and `cd` to it.
4. Connect to Bluemix:

		cf api https://api.stage1.ng.bluemix.net

5. Log into Bluemix:

		cf login -u lauri.ojantakanen@fi.ibm.com
		cf target -o lauri.ojantakanen@fi.ibm.com -s dev
		
6. Compile the Java code and generate the war package using ant.
7. Deploy your app:

		cf push e2esqldb -p libertyDBApp.war

8. Access your app: [http://e2esqldb.stage1.mybluemix.net](http://e2esqldb.stage1.mybluemix.net)
