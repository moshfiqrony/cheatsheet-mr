# Table of content
1. [AJAX Call to a REST API](https://github.com/moshfiqrony/cheatsheet-mr#ajax-call-to-a-rest-api)



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
