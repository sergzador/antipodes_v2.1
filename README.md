# How to run the app:
 1. clone current repository to a local folder
 2. in Terminal navigate to the local folder with docker-compose.yml file
 3. in Terminal execute: ```docker-compose up --build```. This will build and deploy two containers: db and etl
 4. once build is completed, connect to Jupyter Lab by openning in browser ```localhost:8888```
 5. in Jupter Lab, open ```End-to-end-Execution-Demo.ipynb``` file and Run All Cells. This will export data from a web page and write it to DB