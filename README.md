# flask-crud-app
This Repo contains simple flask CRUD operations with mysql

##Dependencies

You should have mysql installed on the localhost in order to test this app ( you can also have it installed on remote and should be updated db_config.py)

Also you should install `flask, flask_table and flask-mysql` use commands `pip3 install flask , pip3 install flask_table , pip3 install flask-mysql`

1. `git clone https://github.com/aleti-pavan/flask-crud-app.git`

2. `cd flask-crud-app\`

3. Create `appdb` and `user_table` for the app. You can either create it manually or choose to use created sql file

     `mysql -uroot < database/user.sql`

    __if you are using rds use following command__

     `mysql -h <rds_accesspoint> -P 3306 -u<username> -p < database/user.sql`


4. If you are using Mac/Linux use `export FLASK_APP=main.py` , if you are using windows `set FLASK_APP=main.py`

5. execute `flask run`

6. curl http://localhost:5000 or you can locate the url into the browser. You should now be able to perform CREATE, READ, UPDATE AND DELETE (CRUD) on the app.
