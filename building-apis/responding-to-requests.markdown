---
title: Building Pleasant APIs - Responding to requests
date: 2021-04-14 23:09:00 -04:00
parent: Building Pleasant APIs
---

Generally when a client makes a request to your API, they expect some sort of response.

A response comes in three parts
- Status Code
- Response Body
- Headers

## Common Successful Responses
The following are some common successful responses, and how they should be formatted

### Creating new resources

### Immediately successful responses

### Responses that will be successful in the future

### Deleting content

## Common Failed Responses
The following are some common unsuccessful responses, and how they should be formatted

#### The client can not access this resource

#### The server can't find the requested resource

#### The server doesn't understand the request

#### Rate limit exceeded

#### Unknown error

## Reference
### Status Codes
#### 200 OK
This status code is used when the client makes a successful request and the server can respond with a relevant response body, unless 201 is more accurate.
* This status code must be accompanied by a response representation. If there is no representation use 204 instead.

#### 201 Created
This status code is used when the client made a successful request and the server created a new resource. 
* This status code must be accompanied by a location header pointing to the new resource
* This status code should be accompanied by the full response representation for the newly created resource

#### 202 Accepted
This status code is used when the server understands the request, it's working on handling the data, but it's not ready yet

#### 204 No Content
This status code is used when the server would return a 200, but no response body.

#### 301 Moved Permanently
#### 302 Found

#### 400 Bad Request
#### 401 Unauthorized
#### 403 Forbidden
#### 404 Not Found
#### 405 Method Not Allowed
#### 406 Not Acceptable
#### 409 Conflict
#### 410 Gone

#### 429 Too Many Requests
#### 451 Unavailable For Legal Reasons

#### 500 Internal Server Error

### Response Body

### Headers
