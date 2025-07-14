

- Apple Pay Merchant Token Management API
-  ErrorResponse 

Object

# ErrorResponse

Information about errors that the API returns in the response body whenever an API request is unsuccessful.

App Store Connect API 1.0.10+

``` source
object ErrorResponse
```

## Properties

`statusCode`

`integer`

 (Required) 

The HTTP status code.

`statusMessage`

`string`

 (Required) 

A description of the error.

`subStatusCode`

`integer`

 (Required) 

A specific sub-status code the system provides to give more context on the type of error.

