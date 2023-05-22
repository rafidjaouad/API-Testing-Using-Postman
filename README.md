# API-Testing-Using-Postman
It's an API testing project where used postman as an API platform and Newman as a command-line Collection Runner for Postman

Postman Project Interface
![Postman](https://github.com/rafidjaouad/API-Testing-Using-Postman/assets/132584373/a566de64-136f-4bed-b089-55c6bf8f7b3b)

Then from the postman 2 files were extracted 
  1: **FlightTicket.postman_collection.json**
  2: **bug7.postman_environment.json**

Now it's time for report generating process.
For that Node.JS and Newman were installed on the system.

**Next Step:**
After installation go to the same diractory where the 2 extracted files are saved and open cmd on that particular folder.

**RUN these 2 commands** 
1st one :  newman run FlightTicket.postman_collection.json -e bug7.postman_environment.json

**Hit ENTER**

2nd one is for the report :  newman run FlightTicket.postman_collection.json -e bug7.postman_environment.json -r cli,html

or 

we can use this command for better interface : newman run FlightTicket.postman_collection.json -e bug7.postman_environment.json -r cli,htmlextra

![CMD 1](https://github.com/rafidjaouad/API-Testing-Using-Postman/assets/132584373/7076e0a7-73c8-4786-a1e2-d82fef0a60f0)

**Now on that particular folder an additional folder will be created called "newman" looked like this**

1: Created by running is command " newman run FlightTicket.postman_collection.json -e bug7.postman_environment.json -r cli,html "

![html](https://github.com/rafidjaouad/API-Testing-Using-Postman/assets/132584373/f352ad1a-be57-4f53-93ff-40b34c2bb75a)

2: Created by running is command " newman run FlightTicket.postman_collection.json -e bug7.postman_environment.json -r cli,htmlextra "

![html extra](https://github.com/rafidjaouad/API-Testing-Using-Postman/assets/132584373/2c6b990c-f57e-4ee0-9ad8-2489b2083567)

If the reports are not generation correctly or says html packages not found try using this commands on globally

**To globally install the htmlextra package:**
 
 npm install -g newman-reporter-html
 
 npm install -g newman-reporter-htmlextra


