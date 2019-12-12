# Table of content
1. [AJAX Call to a REST API](https://github.com/moshfiqrony/cheatsheet-mr#ajax-call-to-a-rest-api)
2. [Delete migrations Django](https://github.com/moshfiqrony/cheatsheet-mr/blob/master/README.md#delete-migrations-django)


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
