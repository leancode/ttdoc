
### timetrex/classes/modules/.* 
All Modules Will Have At Least Two Files <br>
.*Factory.class (They Get Data from ListFactory, and Proccess them Before Returen it to api, and save data to db) 
.*RequestListFactory.class (This For Fetching Data)

### timetrex/classes/modules/api
This Hold All API Routing, They Really Act As Controller (In Laravel) 


### timetrex/classes/modules/plugins
This Folder Hold all Plugins. They Overwrite The Original Class

### timetrex/interface/html5 
This Will Contains All Logic Of Showen UI, It's All About Javascript (backbone, html,css)

### timetrex/includes
Some Global Class That Used To Run The Application.
Like Class Maps, Database Configurations, etc

### timetrex/api
Contains Common Logic That Tells Scripts How To Parse API Requests.
You Don't Have To Touch These Files, Only If You Want For Example, Create A New Way Of Returned Data Like XML 