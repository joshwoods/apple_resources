

- AVFoundation
- AVMetadataGroup
-  items 

Instance Property

# items

The array of metadata items associated with the metadata group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var items: [AVMetadataItem] { get }
```

## Discussion

The `items` array may be empty if no metadata items are associated with this group.

## See Also

### Inspecting the Metadata Group

var uniqueID: String?

The unique identifier for the metadata group.

var classifyingLabel: String?

The classifying label associated with the metadata group.

