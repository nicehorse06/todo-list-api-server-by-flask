# Todo list API server by Flask

## Intro
* Todo list API server by Flask, Celery, SQLAlchemy, Redis, SQLite, gunicorn nginx
* Implement [todo-list-api](https://github.com/nicehorse06/se-job/blob/master/backend/side_project.md#todo-list-api)

## Future features
* Have a RDBS
    * Create a Todo table with IDs, Todos and Done.
* API makes full use of HTTP methods to differentiate actions.
* Add a user system
    * user permissions for the API,
    * only certain accounts can perform certain functions.
* Added login function
    * To obtain `token` for API use authentication
* Added API rate limiter
    * To limit the number of API usage
* Set up a caching system for the API to handle repeated requests.
* Create a replica for DB, read and write separation.
* Concatenate the cash flow so that the API can be charged.
* Implement a load balance system for API
* Implement container settings like `Docker`, `Docker compose`, `Kubernetes`.
* Complete documentation can be referenced, such as Swagger.
* Deployed in public cloud
* Implement the client for the API
* Implement a decentralized system with Queue and solve the problem of race conditions
* Make CLI command to help develop project
    * python manage.py create_db
* Make Golang, Node.js version

## API schema

### POST /tasks
* Create a task.
### GET /tasks
* Read a task.
### GET /tasks/<int>
* Read a tasks list
### PUT /tasks/<int>
* Update a task.
### DELETE /tasks/<int>
* Delete a task.

## ref
* [flask-on-docker](https://testdriven.io/blog/dockerizing-flask-with-postgres-gunicorn-and-nginx)
* [Python Web Flask 實戰開發教學 - SQLAlchemy 與 ORM](https://blog.techbridge.cc/2017/08/12/python-web-flask101-tutorial-sqlalchemy-orm-database-models/)
* [Get started with Docker Compose](https://docs.docker.com/compose/gettingstarted/)
* [mattkohl/docker-flask-celery-redis](https://github.com/mattkohl/docker-flask-celery-redis)
* [Error 99 connecting to localhost:6379. Cannot assign requested address](https://stackoverflow.com/questions/54965291/error-99-connecting-to-localhost6379-cannot-assign-requested-address)
	* 開發環境和正式環境的Redis路徑不一樣
* [Docker Compose ERROR network has active endpoints](https://blog.csdn.net/kinginblue/article/details/78077769)
	* 太久沒有重啟docker server會怪怪

* [[Python] Flask 的 Gunicorn 的 Dcoker 包装方法](https://alphafan.github.io/posts/docker_gunicorn.html)
* [docker-python-gunicorn-nginx](https://github.com/matthieugouel/docker-python-gunicorn-nginx)
* [quokkaproject/docker-gunicorn-supervisor](https://github.com/quokkaproject/docker-gunicorn-supervisor)
* [使用 docker Supervisor 來管理程式](https://philipzheng.gitbooks.io/docker_practice/content/cases/supervisor.html)
* [The Flask Mega-Tutorial Part XVII: Deployment on Linux](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xvii-deployment-on-linux-even-on-the-raspberry-pi)
* [Flask Gunicorn Supervisor Nginx 项目部署小总结](https://gist.github.com/binderclip/f6b6f5ed4d71fa64c7c5)
* [Python Web 部署： 使用 flask + gunicorn + supervisor + nginx](https://juejin.im/post/5a30f7f0f265da43346fe8b5)
* [nicehorse06/flask-movie-list-on-docker](https://github.com/nicehorse06/flask-movie-list-on-docker/tree/master/services/web)
* [Intro what is RESTFUL API 要來介紹什麼是 REST](https://ithelp.ithome.com.tw/articles/10189589)
* [Todo List API by POSTMAN](https://documenter.getpostman.com/view/8858534/SW7dX7JG)
    * good
* [todoist developer](https://developer.todoist.com/guides/#developing-with-todoist)
    * Good to referense
