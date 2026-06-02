# FUTURE_CS_03

# API Security Risk Analysis

## Project Overview

This project focuses on performing an API Security Risk Analysis using Postman on the JSONPlaceholder API.

The objective was to identify potential security risks, analyze API responses, review authentication requirements, evaluate data exposure, and assess error handling mechanisms.

---

## Target API

https://jsonplaceholder.typicode.com/

---

## Tools Used

- Postman
- Browser
- Manual Analysis

---

## Methodology

1. Endpoint Enumeration
2. Response Analysis
3. Authentication Review
4. Data Exposure Assessment
5. Error Handling Analysis
6. POST Request Testing
7. API Response Validation

---

## API Endpoints Tested

### GET /users

Endpoint:

https://jsonplaceholder.typicode.com/users

Result:

- Status Code: 200 OK
- User data returned successfully
- No authentication required

Finding:

**No Authentication Required**

Severity: Medium

---

### GET /posts

Endpoint:

https://jsonplaceholder.typicode.com/posts

Result:

- Status Code: 200 OK
- Post data returned successfully
- Publicly accessible endpoint

Finding:

**Public Data Exposure**

Severity: Low

---

### GET /admin

Endpoint:

https://jsonplaceholder.typicode.com/admin

Result:

- Status Code: 404 Not Found

Finding:

**Proper Error Handling**

Severity: Informational

---

### POST /posts

Endpoint:

https://jsonplaceholder.typicode.com/posts

Result:

- Status Code: 201 Created
- Resource created successfully

Finding:

**API Accepts Data Submission**

Severity: Informational

---

## Risk Summary

| Finding | Severity |
|----------|----------|
| No Authentication Required | Medium |
| Public Data Exposure | Low |
| Proper Error Handling | Informational |
| API Accepts Data Submission | Informational |

---

## Recommendations

- Implement JWT Authentication
- Apply Role-Based Access Controls
- Limit Public Data Exposure
- Validate User Input
- Implement Rate Limiting
- Monitor API Activity

---

## Screenshots

The Screenshots folder contains:

- Get_Users.png
- Get_Posts.png
- Invalid_Endpoint.png
- Post_Request.png

---

## Conclusion

The assessment identified publicly accessible endpoints and the absence of authentication controls. Proper error handling was observed, and recommendations were provided to improve API security in production environments.

This project helped develop practical skills in API testing, endpoint analysis, risk identification, and cybersecurity reporting.
