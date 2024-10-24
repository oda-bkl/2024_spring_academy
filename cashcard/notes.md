# Notes

## HTTP vs REST
Operation | HTTP Method | Response Status Code
----------|--------------|--------------------
Create    | POST        | 201 Created
Read      | GET         | 200 OK
Update    | PUT         | 204 No Content or 201 Created
Delete    | DELETE      | 204 No Content


## Repository Pattern
- A repository is a class that is responsible for abstracting the data layer from the rest of the application.

## Layered Architecture
1. Presentation Layer  
API Clients, Web Browsers, Mobile Apps  
1. Application Layer  
Controller, Business Logic
1. Data Access Layer  
Repository (Abstraction for any Database), Database

## HTTP 201 CREATED
- Needs a Location header with the URI of the newly created resource.

## CSRF
Cross-Site Request Forgery
- When should you use CSRF protection? Our recommendation is to use CSRF protection for any request that could be processed by a browser by normal users. If you are only creating a service that is used by non-browser clients, you will likely want to disable CSRF protection.


## Links
[HTTP Standard RFC 9110](https://www.rfc-editor.org/rfc/rfc9110)
