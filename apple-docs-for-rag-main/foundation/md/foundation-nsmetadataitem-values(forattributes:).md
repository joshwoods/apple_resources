

- Foundation
- NSMetadataItem
-  values(forAttributes:) 

Instance Method

# values(forAttributes:)

Returns a dictionary containing the key-value pairs for the attribute names specified by a given array of keys.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func values(forAttributes keys: [String]) -> [String : Any]?
```

## Parameters 

`keys`  

An array containing `NSString` objects that specify the names of a metadata attributes. See the “Constants” section for a list of possible keys.

## Return Value

A dictionary containing the key-value pairs for the attribute names specified by `keys`.

## See Also

### Getting Item Attributes

var attributes: [String]

An array containing the attribute keys for the metadata item’s values.

func value(forAttribute: String) -> Any?

Returns the receiver’s metadata attribute name specified by a given key.

