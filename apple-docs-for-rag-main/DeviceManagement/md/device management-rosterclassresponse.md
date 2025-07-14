

- Device Management
-  RosterClassResponse 

Object

# RosterClassResponse

The response that contains a list of classes.

Device Assignment ServicesVPP License Management

``` source
object RosterClassResponse
```

## Properties

`classes`

`[`RosterClass`]`

An array of classes, sorted in lexical order by a class `source_system_identifier`. The organization must provide this identifier to Apple.

`cursor`

`string`

A hex string that should be used for the next request to paginate. This field data type has a maximum length of 512 UTF-8 characters.

`more_to_follow`

`boolean`

Indicates whether the request’s limit and cursor values resulted in only a partial list of classes. If `true`, the MDM server should then make another request (starting from the newly returned cursor) to obtain additional records.

## See Also

### Request and Response

object RosterRequest

The request for a list of classes.

