Hub Planner API
===

Welcome to the Hub Planner API. The Hub Planner API provides programmatic access to the following [Sections](https://github.com/hubplanner/API/tree/master/Sections)

* [Projects](https://github.com/hubplanner/API/blob/master/Sections/project.md)
* [Resources](https://github.com/hubplanner/API/blob/master/Sections/resource.md)
* [Timesheets](https://github.com/hubplanner/API/blob/master/Sections/timesheets.md)
* [Bookings](https://github.com/hubplanner/API/blob/master/Sections/bookings.md)
* [Events](https://github.com/hubplanner/API/blob/master/Sections/events.md)
* [Holidays](https://github.com/hubplanner/API/blob/master/Sections/holidays.md)
* [Groups](https://github.com/hubplanner/API/blob/master/Sections/groups.md)
* [Milestones](https://github.com/hubplanner/API/blob/master/Sections/milestones.md)

You can use the API to integrate Hub Planner with your own third party applications or generally integrate with your existing back-office setup.

##API Support
The API is in beta status which means it is a fully functioning API but there maybe some unforeseen bugs that we will iron out as soon as we get receive them.

If you have a question about using the API or have noticed an error or omission in the documentation. Please feel free to open an [issue](https://github.com/hubplanner/API/issues) on GitHub with your question and we will attend to it.

If you have any direct implementation issues, please contact the tech team at the following address hello@hubplanner.com and add API as as the Subject. 

##API Updates and Changes
We will be managing the API via GitHub, so please watch the Hub Planner API repository to receive email notification of updates to the API documentation. 

##Sharing
If you've built something interesting with the Hub Planner API, made a wrapper for a certain code language or integrated with a third party software you would like to share or think will help others, then please let us know at hello@hubplanner.com

##API Data Formats
Hub Planner API is a RESTful API that uses HTTP requests and returns JSON for all responses. 

All URLs start with the root URL: 

```
https://api.hubplanner.com/v1/
```
Content-Type and Accept must be defined in the header of all requests. 

```
GET resource/123
Accept: application/json
Content-Type: application/json
```

Please note that all requests to the Hub Planner API must be made over HTTPS.

##User Agent Identification
Remember to write your application carefully. In case of abuse you may be blocked, disallowing further API access. As an act of courtesy, please provide User-Agent strings denoting your application.

`User-Agent: My Hub Planner Import App (my-name@my-email.com)`

##Authentication

Hub Planner API is authenticated with a OAuth 2.0 Bearer Token.

You must supply an Authorization header with the token for all requests. 

`Authorization: xxx`

You must enable API access and generate your API key and in order to use the Hub Planner API. The API key is available in All Accounts with Administrator privileges and higher. To generate your API key and enable the API login to your Hub Planner account and navigate to 

`Settings -> API`

Here you can generate your key for different rights and enable access.

There are 2 types of API keys you can generate.
* Read Only
* Read & Write

Please note if you decide to disable access to the API. All API access will be revoked for all generated keys. The generated keys should be considered as sensitive as passwords and must not be shared or distributed to untrusted parties.

##Examples
Below we are lising some integration examples you can follow. Please let us know if you would like to add an example to this list. hello@hubplanner.com

* [harvest](https://github.com/hubplanner/API/tree/master/Examples/harvest)
