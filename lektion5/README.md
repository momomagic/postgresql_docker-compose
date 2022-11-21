# Jupyter notebook 

### Working with docker compose

```bash
cd folder_where_postgres-sql-docker-compose
git pull 
cd lektion5
docker-compose up -d
docker-compose logs 
```
 * Jupyter notebook will be exposed to 127.0.0.1:8089/
 * Copy link in logs starting with 127.0.0.1:8888/....   and replace 8888 with 8089
 * Look for jupyter notebook in /opt/jupyter/

### Working without docker-compose
```bash
cd folder_where_postgres-sql-docker-compose
git pull
cd lektion5
```
* Open jupyter notebook in visual studio code 
* Run first cell up to install library
* If you have issues with installing library follow the following 
   ```bash
  python -m venv venv  #create virtual environment for hadling libraries
  pip install --user ipykernel #install ipykernel to manage jupyter kernel
  python -m ipykernel install --user --name=venv  #adding venv to jupyter as kernel