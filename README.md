# Open-Elevation

[https://open-elevation.com](https://open-elevation.com)

A free and open-source elevation API.

**Open-Elevation** is a free and open-source alternative to the [Google Elevation API](https://developers.google.com/maps/documentation/elevation/start) and similar offerings.

This service came out of the need to have a hosted, easy to use and easy to setup elevation API. While there are some alternatives out there, none of them work out of the box, and seem to point to dead datasets. <b>Open-Elevation</b> is [easy to setup](https://github.com/Jorl17/open-elevation/blob/master/docs/host-your-own.md), has its own docker image and provides scripts for you to easily acquire whatever datasets you want. We offer you the whole world with our [public API](https://github.com/Jorl17/open-elevation/blob/master/docs/api.md).

If you enjoy our service, please consider [donating to us](https://open-elevation.com#donate). Servers aren't free :)

**API Docs are [available here](https://github.com/Jorl17/open-elevation/blob/master/docs/api.md)**

You can learn more about the project, including its **free public API** in [the website](https://open-elevation.com)

## Donations

Please consider donating to keep the public API alive. This API is **used by millions of users every day** and it costs money to keep running!

You can donate [by following this link](https://www.open-elevation.com/#donate).

### Examples

```shell
http://0.0.0.0:8080/api/v1/lookup?locations=10,10|20,20|41.161758,-8.583933
http://0.0.0.0:8080/api/v1/lookup?locations=0.552196,22.353005
https://api.open-elevation.com:8080/api/v1/lookup?locations=20.799,5.261
curl 'https://api.open-elevation.com/api/v1/lookup?locations=20.799,5.261'
{"results":[{"latitude":20.799,"longitude":5.261,"elevation":606.0}]}%
http://0.0.0.0:8080/api/v1/lookup?locations=20.799,5.261

curl -X POST \
   http://0.0.0.0:8080/api/v1/lookup \
  -H 'Accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{
	"locations":
	[
		{
			"latitude": 45.39055633480109,
			"longitude": -121.79312499371613
		},
		{
			"latitude": 45.38877348862923,
			"longitude": -121.78337657913022
		},
		{
			"latitude": 45.38800340088005,
			"longitude": -121.77320812026105
		},
		{
			"latitude": 45.38727306529623,
			"longitude": -121.76359035102229
		},
		{
			"latitude": 45.382780731109875,
			"longitude": -121.75289621930827
		},
		{
			"latitude": 45.381310938059556,
			"longitude": -121.74327840878331
		},
		{
			"latitude": 45.37928656248073,
			"longitude": -121.73187872216528
		},
		{
			"latitude": 45.377221727224736,
			"longitude": -121.7221113727771
		},
		{
			"latitude": 45.37607693840755,
			"longitude": -121.71482376380962
		},
		{
			"latitude": 45.37385812416366,
			"longitude": -121.70538213558189
		},
		{
			"latitude": 45.37445146184737,
			"longitude": -121.6956484591046
		},
		{
			"latitude": 45.36544568665036,
			"longitude": -121.69529051169866
		},
		{
			"latitude": 45.35865602693869,
			"longitude": -121.68780892935683
		},
		{
			"latitude": 45.34493718717218,
			"longitude": -121.67781906028222
		},
		{
			"latitude": 45.335781774449146,
			"longitude": -121.6718580095469
		},
		{
			"latitude": 45.325893390152686,
			"longitude": -121.66874225753043
		},
		{
			"latitude": 45.31661685642371,
			"longitude": -121.66023442494942
		},
		{
			"latitude": 45.30789891138332,
			"longitude": -121.65191203530986
		},
		{
			"latitude": 45.29644891952182,
			"longitude": -121.64127947995071
		}
	]
}'
```

