# Vagrant RapidPro
```
vagrant up
vagrant ssh
pyenv install 3.7.0
pyenv global 3.7.0
nvm install 10
cd /vagrant
git clone https://github.com/rapidpro/rapidpro
cd rapidpro/temba
ln -s settings.py.dev settings.py
pyenv virtualenv env
pyenv activate env
cd ..
pip install -r pip-freeze.txt
python manage.py migrate
npm install
npm install less -g
npm install coffeescript -g
python manage.py createsuperuser
python manage.py runserver 0.0.0.0:8000
```

Start Mailroom
In another terminal in this project folder
```
vagrant ssh
wget https://github.com/nyaruka/mailroom/releases/download/v5.3.4/mailroom_5.3.4_linux_amd64.tar.gz
mkdir mailroom
tar -xvf mailroom_5.3.4_linux_amd64.tar.gz -C mailroom
cd mailroom
./mailroom
```


