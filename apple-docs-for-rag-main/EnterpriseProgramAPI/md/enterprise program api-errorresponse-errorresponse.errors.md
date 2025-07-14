

- Enterprise Program API
- ErrorResponse
-  ErrorResponse.Errors 

Object

# ErrorResponse.Errors

The details about an error that are returned when an API request isn’t successful.

``` source
object ErrorResponse.Errors
```

## Properties

`code`

`string`

 (Required) 

A machine-readable code indicating the type of error. The code is a hierarchical value with levels of specificity separated by the ‘`.`’ character. This value is parseable for programmatic error handling in code.

`status`

`string`

 (Required) 

The HTTP status code of the error. This status code usually matches the response’s status code; however, if the request produces multiple errors, these two codes may differ.

`id`

`string`

The unique ID of a specific instance of an error, request, and response. Use this ID when providing feedback to or debugging issues with Apple.

`title`

`string`

 (Required) 

A summary of the error. Do not use this field for programmatic error handling.

`detail`

`string`

 (Required) 

A detailed explanation of the error. Do not use this field for programmatic error handling.

`source`

`*`

One of two possible types of values: `source.Parameter`, provided when a query parameter produced the error, or `source.JsonPointer`, provided when a problem with the entity produced the error.

Possible types: JsonPointer`, `Parameter

`links`

ErrorLinks

`meta`

ErrorResponse.Errors.Meta

## Attributes 

Possible types:

## Discussion

Use the `code` parameter for programmatic error handling. See Parsing the Error Response Code for more information. For more information about using the `source` parameter, see Pinpointing the Location of Errors.

## Topics

### Objects

object JsonPointer

An object that contains the JSON pointer that indicates the location of the error.

object Parameter

An object that contains the query parameter that produced the error.

object ErrorResponse.Errors.Meta

An object that contains the error itself or associated errors.

