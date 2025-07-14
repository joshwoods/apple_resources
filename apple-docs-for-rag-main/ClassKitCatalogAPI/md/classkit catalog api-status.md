

- ClassKit Catalog API
-  Status 

Dictionary

# Status

The state of a request that the API previously accepted, but didn’t complete right away.

ClassKit 1.0+

``` source
object Status
```

## Properties

`location`

`string`

The URL used to retrieve this status.

`state`

`string`

The state of the request.

Possible Values: `pending, inProgress, complete, error`

`teamId`

`string`

The identifier of the team associated with this status.

`statusId`

`string`

The unique value that identifies this status.

`error`

Status.Error

Information that the system provides for a request that fails.

`statusCode`

`string`

A response code that indicates the outcome of the request.

## Attributes 

Possible types:

## Topics

### Errors

object Status.Error

Information that explains why a request failed.

## See Also

### Retrieving Status

Get Status

Fetch the status of an operation that you initiated earlier.

