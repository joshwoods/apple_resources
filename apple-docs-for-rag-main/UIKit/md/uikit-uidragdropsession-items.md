

- UIKit
- UIDragDropSession
-  items 

Instance Property

# items

An array of drag items in the drag session or drop session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var items: [UIDragItem] { get }
```

**Required**

## Discussion

The drag item’s NSItemProvider object doesn’t load the data for the item until the drop interaction happens. However, before the interaction happens, you can get the item’s registered type identifiers and metadata. The data is available to you only in the drop interaction delegate’s dropInteraction(_:performDrop:) method.

## See Also

### Checking for drag items

func canLoadObjects(ofClass: any NSItemProviderReading.Type) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session can create an instance of the specified class.

**Required** Default implementation provided.

func hasItemsConforming(toTypeIdentifiers: [String]) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session conforms to at least one of the specified UTIs.

**Required**

