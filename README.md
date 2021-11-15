#FastAPI SQL pyodbc POC
Update app.py with your connection string & use the following startup command on Azure for gunicorn:
```
gunicorn --bind=0.0.0.0 --timeout 600 -w 4 -k uvicorn.workers.UvicornWorker api:app
```
> / - Returns SQL Server Info
> /drivers - return drivers avaliable