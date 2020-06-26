## Overview
-  [DPX Technology](#dpx-general)
    -  [Architecture](#architecture)
    -  [Technical Stacks](#tech-stacks)
-  [DPX Connect Api](#connect-api)
    -  [Overview](#connect-api)
    -  [Authentication](#connect-api-auth)
    -  [Example Request](#connect-api-request)
    -  [V1 Specification](#connect-api-specification)
    -  [Changelog](#connect-api-changelog)    

### <span id="dpx-general"></span>DPX Technology
DPX is financial pricing software built on the modern web application architecture and technical stacks.

You can find more product information from [Brilliance website](https://bxfin.com/).

#### <span id="architecture"> Architecture
- SPA (Single Page Application)
- RESTful API
- Layered Architecture

#### <span id="tech-stacks"> Technical Stacks
- Asp.NET Core
- Angular
- Entity Framework Core
- SQL Server
- Cloud Data Storage

### <span id="connect-api"></span>DPX Connect API
DPX Connect API provides RESTful api for pricing integration. You can use the API to request pricing integration tasks with standard GET,POST,PUT,DELETE http methods.

- Latest Version : Connect Api V1

#### <span id="auth"> Authentication
To access the APIs, the client system should include `x-api-key` in the request HTTP header.

You can get the api-key from tenant admin page or your system admin.

#### <span id="connect-api-request"> Example Request

To request, you need to include the following http headers.

- `Content-Type` : application/json
- `x-api-key` : -your-api-key

Refer the Postman example to request echo endpoint

[GET] `/connect/test/echo`

![alt text](images/Connect_APIs_1.PNG "API Key based request")

#### <span id="connect-api-specification"> API V1 Specification

DPX provides public Swagger documents for the latest API specification.

- <a href="https://rc.dpxpricing.com/swagger" target="_blank">Connect API V1 document</a>


#### <span id="connect-api-changelog"> API Changelog
- [Change Log](ApiChangeLog.md)