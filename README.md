# cheatsheet-mr

## AJAX Call to a REST API

```javascript
$.ajax({
	type: 'GET',
	url: 'http://localhost:8000/api/user/profile/',
	beforeSend: function (xhr, settings) {
        xhr.setRequestHeader("Authorization", 'TOKEN 064239741b0f68c868365a5e504169fcf2499a26');
    },
	success: function(data){
		console.log(data)
	}
}
```
