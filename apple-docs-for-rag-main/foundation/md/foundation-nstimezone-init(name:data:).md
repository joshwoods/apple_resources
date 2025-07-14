

- Foundation
- NSTimeZone
-  init(name:data:) 

Initializer

# init(name:data:)

Initializes a time zone with a given identifier and time zone data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    name tzName: String,
    data aData: Data?
)
```

## Parameters 

`tzName`  

The identifier for the time zone. Providing `nil` for this parameter raises an invalid argument exception.

`aData`  

This parameter is ignored.

## Discussion

As of macOS 10.6, the underlying implementation of this method has been changed to ignore the specified `data` parameter.

Important

You should not use this method. Instead, use init(name:) to initialize a time zone object with a given name.

## See Also

### Creating Time Zones

init?(name: String)

Returns a time zone initialized with a given identifier.

convenience init?(abbreviation: String)

Returns the time zone object identified by a given abbreviation.

convenience init(forSecondsFromGMT: Int)

Returns a time zone object offset from Greenwich Mean Time by a given number of seconds.

class var knownTimeZoneNames: [String]

Returns an array of strings listing the IDs of all the time zones known to the system.

class var abbreviationDictionary: [String : String]

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

