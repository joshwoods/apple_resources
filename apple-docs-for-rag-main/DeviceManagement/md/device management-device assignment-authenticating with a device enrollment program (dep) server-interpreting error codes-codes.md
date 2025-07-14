

- Device Management
- Device Assignment
- Authenticating with a Device Enrollment Program (DEP) Server
-  Interpreting Error Codes 

Article

# Interpreting Error Codes

Interpret the error codes you might encounter or that can happen during authentication.

## Overview

Authentication errors are either a `400`, `401`, or `403` error code.

An `HTTP 400 Bad Request` error indicates one of the following:

- Unsupported OAuth parameters

- Unsupported signature method

- Missing required authorization parameter

- Duplicated OAuth protocol parameter

An `HTTP 401 Unauthorized` error indicates one of the following:

- Invalid consumer key

- Invalid or expired token

- Invalid signature

- Invalid or already-used nonce

An `HTTP 403 Forbidden` error indicates one of the following:

- The MDM server, or the MDM server’s consumer key/token does not have access to perform the specific request. In this case, the request body contains `ACCESS_DENIED`.

- The organization has not accepted the latest terms and conditions of the program. In this case, the request body contains `T_C_NOT_SIGNED`.

## See Also

### Examples and Error Codes

Examining Server Tokens

View sample encrypted and unencrypted tokens to verify your server tokens are in the right format.

