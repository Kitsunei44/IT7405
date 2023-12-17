Start Anaconda Prombt-
Make Virtual Environment:
	cd ...\Project\main
	conda create --name Project django
	activate Project
pip list:
	- django 3.1
	- djongo 1.3.6
	- pymongo 3.12.1
	- pytz 2022.6
	- sqlparse 0.2.4
	- pillow

//Setup for database importing//

In MongoDB COMPASS:
	create a Database with the name (mainProject) collection name(item)

In ANACONDA PROMBT:
	python manage.py makemigrations
	python manage.py migrate

In MongoDB COMPASS:
	--All JSON Files found in MongoDBJSONS Folder--
	Import mainProject.home_gear.json into home_gear
	Import mainProject.home_vehicle.json into home_vehicle

//Starting Up//

In ANACONDA PROMBT:
	python manage.py createsuperuser
	python manage.py makemigrations
	python manage.py migrate
	python manage.py runserver