

- UIKit
- UIDragDropSession
-  hasItemsConforming(toTypeIdentifiers:) 

Instance Method

# hasItemsConforming(toTypeIdentifiers:)

Returns a Boolean value that indicates whether at least one drag item in the session conforms to at least one of the specified UTIs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func hasItemsConforming(toTypeIdentifiers typeIdentifiers: [String]) -> Bool
```

**Required**

## Parameters 

`typeIdentifiers`  

An array of uniform type identifier (UTI) strings.

## Return Value

true if a drag item in the session conforms to any UTI in the specified array; otherwise, false.

## See Also

### Checking for drag items

func canLoadObjects(ofClass: any NSItemProviderReading.Type) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session can create an instance of the specified class.

**Required** Default implementation provided.

var items: [UIDragItem]

An array of drag items in the drag session or drop session.

**Required**

