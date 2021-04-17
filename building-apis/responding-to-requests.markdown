---
title: Building Pleasant APIs - Responding to requests
date: 2021-04-14 23:09:00 -04:00
parent: Building Pleasant APIs
---

Generally when a client makes a request to your API, they expect some sort of response.

An HTTP response comes in three parts
- The status Code
- A response Body
- A collection of headers

First we'll walk through a series of common successful and unsuccessful responses. Once you've read those, feel free to jump right to the [detailed reference](#reference).

## Common Successful Responses
If everything is O.K. with the clients request, the server must return one of the following successful responses.

### Creating new resources

### Immediately successful responses

### Responses that will be successful in the future

### Deleting content

## Common Failed Responses
If the server chooses to reject the request for any reason, they must return one of the following responses.

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
