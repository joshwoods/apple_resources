

- UIKit
- UIDragDropSession
-  canLoadObjects(ofClass:) 

Instance Method

# canLoadObjects(ofClass:)

Returns a Boolean value that indicates whether at least one drag item in the session can create an instance of the specified class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func canLoadObjects(ofClass aClass: any NSItemProviderReading.Type) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`aClass`  

A class conforming to the NSItemProviderReading protocol.

## Return Value

true if at least one drag item in the session can create an instance of the specified class; otherwise, false.

## Default Implementations

### UIDragDropSession Implementations

func canLoadObjects&lt;T>(ofClass: T.Type) -> Bool

## See Also

### Checking for drag items

func hasItemsConforming(toTypeIdentifiers: [String]) -> Bool

Returns a Boolean value that indicates whether at least one drag item in the session conforms to at least one of the specified UTIs.

**Required**

var items: [UIDragItem]

An array of drag items in the drag session or drop session.

**Required**

