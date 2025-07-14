

- Device Management
-  RosterClassLocationResponse 

Object

# RosterClassLocationResponse

The response that contains a list of locations.

Device Assignment ServicesVPP License Management

``` source
object RosterClassLocationResponse
```

## Properties

`cursor`

`string`

A hex string that should be used for the next request to paginate. This field data type has a maximum length of 512 UTF-8 characters.

`locations`

`[`RosterLocation`]`

Provides information about locations, sorted in lexical order by a location `source_system_identifier`. The organization must provide this identifier to Apple.

`more_to_follow`

`boolean`

Indicates whether the request’s limit and cursor values resulted in only a partial list of classes. If `true`, the Mobile Device Management server should then make another request (starting from the newly returned cursor) to obtain additional records.

