

- Core Data
- NSPropertyDescription
-  isIndexedBySpotlight 

Instance Property

# isIndexedBySpotlight

A Boolean value that indicates whether Core Data adds the property’s value to the Core Spotlight index.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isIndexedBySpotlight: Bool { get set }
```

## Discussion

Important

If you set this property to true for a property description that describes a relationship, you must override attributeSet(for:) in your Core Spotlight delegate and return the necessary set of attributes. Core Data doesn’t automatically infer indexable information for relationships.

You can also set this property using the Index in Spotlight attribute in the Attributes inspector of the Core Data model editor.

## See Also

### Specifying Spotlight Support

var isStoredInExternalRecord: Bool

A Boolean value that indicates whether to write the property’s data in an external record file that corresponds to the managed object.

Deprecated

