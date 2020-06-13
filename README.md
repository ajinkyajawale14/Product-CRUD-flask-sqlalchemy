# Product-CRUD-flask-sqlalchemy

Flask CRUD application using SQL Alchemy and SQlite DB

### CRUD - Flask rest api implementation in python with SQLite database (RDBMS)

Intructions:

create python3 venv

	1.1) sudo apt install python3-venv
	
	1.2) python3 -m venv my-project-env
	
	1.3) source my-project-env/bin/activate

install dependencies

pip install -r requirements.txt

( -r will remove previous package if present and install package version metioned in requirement.txt file )

install DB Browser for SQLite for better understanding of your DB maintain it well :)

sudo apt-get install sqlitebrowser

4)create a SQLite Database

  #python3

  	#database models
  	class User(db.Model):
    	  __tablename__ = 'users'
      	# db fields ...
	
	# db Schema
	
	# Product Schema
	
	class ProductSchema(ma.Schema):
  		class Meta:
    		fields = ('id', 'name', 'description', 'price', 'qty')

	# Init schema
	
	product_schema = ProductSchema(strict=True)	
	  
flask run :)
