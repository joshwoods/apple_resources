

- Device Management
-  Error 

Object

# Error

Information about an error that occurred while processing a request.

Device Assignment ServicesVPP License Management

``` source
object Error
```

## Properties

`code`

`string`

 (Required) 

The specific code for the underlying cause of the error.

`detail`

`string`

More detailed information about the cause of the error, intended to help identify possible resolutions.

`id`

`string`

 (Required) 

The identifier of the error, mapping to the occurrence.

`source`

Error.Source

An object containing a reference to the source of the error.

`status`

`string`

 (Required) 

The HTTP status code the error maps to.

`title`

`string`

 (Required) 

A developer-friendly title for the error.

## Topics

### Related Objects

object Error.Source

An object that represents the source of an error.

## See Also

### Handling errors

Interpreting HTTP status codes

Interpret error codes the API might return when executing a request.

