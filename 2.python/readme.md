

|Commund|note|
|---|---|
|sudo apt install python3-pip python3-dev nginx| |
|sudo pip3 install virtualenv| |
|git clone https://github.com/mavenium/PyEditorial |# clone the project|
|cd PyEditorial	|# Run the project-|
|virtualenv -p python3 .venv|# Run the project--|
|source .venv/bin/activate|# Run the project---|
|pip install -r requirements.txt|# Run the project--|
|python manage.py makemigrations|# Run the project---|
|python manage.py migrate|# Run the project|
|python manage.py collectstatic|# Run the project|
|python manage.py runserver|# Run the project|
|deactivate|


