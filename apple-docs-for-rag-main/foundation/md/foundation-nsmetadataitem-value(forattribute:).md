

- Foundation
- NSMetadataItem
-  value(forAttribute:) 

Instance Method

# value(forAttribute:)

Returns the receiver’s metadata attribute name specified by a given key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forAttribute key: String) -> Any?
```

## Parameters 

`key`  

The name of a metadata attribute. See the “Constants” section for a list of possible keys.

## Return Value

The receiver’s metadata attribute name specified by `key`.

## See Also

### Getting Item Attributes

var attributes: [String]

An array containing the attribute keys for the metadata item’s values.

func values(forAttributes: [String]) -> [String : Any]?

Returns a dictionary containing the key-value pairs for the attribute names specified by a given array of keys.

