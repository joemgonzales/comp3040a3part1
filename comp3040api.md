# Parks in Manitoba

## API Description

A simple API to get information about parks in Manitoba. It returns information about the operating hours and available amenities for convenience.
There are plenty of parks and it is hard to keep track of them all, which this API serves to assist with.

## Endpoints

There is a single endpoint which can be accessed with a GET request to **https://api.parks-manitoba.ca/json**.

### Parameters

* **name**(string) - name of the park
* **month**(int) - number of the month in a year
* **formatted**(int) - 0 or 1 (1 is default). Hours of operation in response will be expressed following ISO 8601


## Description of resources

```
{
	"information":
	{
		"park_name": full name of the park
		"hours_of_operation": unformatted or formatted, based on month of year
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

**Request**

```https://api.parks-manitoba.ca/json?name=whiteshell&month=6&formatted=1```  
**Response**

```
{
	"information":
	{
		"park_name": "whiteshell"
		"hours_of_operation": "6:00 AM - 4:30 PM"
		"amenities":
		{
			"beach": yes
			"fishing": yes
			"hiking_trail": yes
			"picnic_area": yes
			"golf": yes
		}
	}
}
```
