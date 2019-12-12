# Table of content
1. [AJAX Call to a REST API](https://github.com/moshfiqrony/cheatsheet-mr/blob/master/README.md#ajax-call-to-a-rest-api)
2. [Delete migrations Django](https://github.com/moshfiqrony/cheatsheet-mr/blob/master/README.md#delete-migrations-django)
2. [Git sync with upstream](https://github.com/moshfiqrony/cheatsheet-mr/blob/master/README.md#git-sync-with-upstream)


## AJAX Call to a REST API

```javascript
$.ajax({
	type: 'GET',
	url: 'http://localhost:8000/api/user/profile/',
	beforeSend: function (xhr, settings) {
        xhr.setRequestHeader("Authorization", 'TOKEN your_token');
    },
	success: function(data){
		console.log(data)
	}
}
```

## Delete migrations Django
```terminal
find . -path "*/migrations/*.py" -not -name "__init__.py" -delete
find . -path "*/migrations/*.pyc"  -delete
```


## Git sync with upstream
```terminal
git remote add upstream https://github.com/datafordecisions/cultivate.git

git fetch upstream

git merge upstream/master

git push origin master
```


## Postgres SQL username Reset
At first run the following command 
```terminal
sudo -u postgres psql
```
it will open the postsgressql console then just simply type the following command
```terminal
ALTER USER postgres PASSWORD '1234';
```

## If Permission Denied For React Native
This happened because of  sudo permission. simply run the app under sudo permission
``` terminal
sudo su
react-native run-android
```

## How to make htdocs sudo permission
```
sudo chmod -R 777 ./htdocs
```

### Virtual Environment with Python 3.6
```
virtualenv --python=python3.6 myvenv
```

## Remove Node JS

```
sudo apt-get purge nodejs

sudo apt-get autoremove
```

## Node Js Install Fron tra.gz file 
Extract the file and rename to node and run the command from same directory

```
sudo cp -r node/{bin,include,lib,share} /usr/

```


## Lock resource unavailable
```
sudo rm /var/lib/apt/lists/lock


sudo rm /var/cache/apt/archives/lock


sudo rm /var/lib/dpkg/lock
```

## Node Update Procedure
```
sudo apt-get update


sudo apt-get install curl


curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -



sudo apt-get install nodejs
```

## ADV is not working for React Native Android App
```
sudo apt-get update
sudo apt-get install adb
react-native run-android
```
