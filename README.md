# About the project

This is a DataEngineering project.
The project is to extract the data from the amazon and store it in a database.

# Technology used

Python,Docker,Apache Airflow,PgAdmin

# amazon_books

PS C:\Users\Lenovo\Desktop\amazon_books> python -m venv venv  #To create virtual folder
PS C:\Users\Lenovo\Desktop\amazon_books> .\venv\Scripts\activate  #To activate virtual environment
(venv) PS C:\Users\Lenovo\Desktop\amazon_books>

# apache airflow setup 

1.To setup Apache Airflow -> Link :- https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html
2.First open the docker container in the desktop.
3.In the terminal type -> docker compose up
4.To open localhost -> http://localhost:8081 and username - airflow and password - airflow 
5.C:\Program Files\PostgreSQL\16\bin
6.To stop all the services -> docker compose down
7.Then to run airflow to initialize database -> docker compose up airflow-init
8.To get the IP address of the container -> docker inspect 3a2b307fc1f8202c9aca0bd8f34dd3881efa25bcc619d7345a03426dcfb06311

# To sign in to pg-admin

After successfully running -->> docker compose up 
Then i have to run -->> [localhost:5050](http://localhost:5050/login?next=/browser/) for opening of pgAdmin 
Id -->> admin@admin.com  and password -->> root

Then to enter into the server of pg_admin:-
ps_db -->> password is airflow...

# To run the query in pg-admin

query -->> select * from books order by price 


Installed airflow on Docker
Installed postgres and pgadmin
Created DAG