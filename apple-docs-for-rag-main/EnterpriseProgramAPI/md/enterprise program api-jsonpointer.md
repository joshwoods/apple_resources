

- Enterprise Program API
-  JsonPointer 

Object

# JsonPointer

An object that contains the JSON pointer that indicates the location of the error.

``` source
object JsonPointer
```

## Properties

`pointer`

`string`

 (Required) 

A JSON pointer that indicates the location in the request entity where the error originates.

## Attributes 

Possible types:

## Discussion

In some cases, the JSON pointer may indicate an element that isn’t in the request entity, but should be. For more information about JSON pointers, see the RFC 6901 proposed standards document.

## See Also

### Objects

object Parameter

An object that contains the query parameter that produced the error.

object ErrorResponse.Errors.Meta

An object that contains the error itself or associated errors.

