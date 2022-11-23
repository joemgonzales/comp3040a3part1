# Parks in Manitoba

## API Description

A simple API to get information about Parks in Manitoba.

## Endpoints

There is a single endpoint which can be accessed with a GET request to **https://api.parks-manitoba.ca/json**.

## Description of resources

```
{
	"information":
	{
		"park_name": full name of the park
		"hours_of_operation": 
		"amenities":
		{
			"beach": yes/no
			"fishing": yes/no
			"hiking_trail": yes/no
			"picnic_area": yes/no
			"golf": yes/no
		}
	}
}
```

## Sample request with sample response

*Request*
```https://api.parks-manitoba.ca/json?name=whiteshell&month=6&formatted=1```  
*Response*
