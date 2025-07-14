

- Foundation
- NSMetadataItem
-  attributes 

Instance Property

# attributes

An array containing the attribute keys for the metadata item’s values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var attributes: [String] { get }
```

## Discussion

This property contains an array of attribute keys, representing the values available from this metadata item. For a list of possible keys, see `Attribute Keys`.

## See Also

### Getting Item Attributes

func value(forAttribute: String) -> Any?

Returns the receiver’s metadata attribute name specified by a given key.

func values(forAttributes: [String]) -> [String : Any]?

Returns a dictionary containing the key-value pairs for the attribute names specified by a given array of keys.

