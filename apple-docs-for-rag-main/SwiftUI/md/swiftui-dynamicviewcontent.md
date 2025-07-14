

- SwiftUI
-  DynamicViewContent 

Protocol

# DynamicViewContent

A type of view that generates views from an underlying collection of data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol DynamicViewContent : View
```

## Topics

### Managing the data

var data: Self.Data

The collection of underlying data.

**Required**

associatedtype Data : Collection

The type of the underlying collection of data.

**Required**

### Responding to updates

func onDelete(perform: Optional&lt;(IndexSet) -> Void>) -> some DynamicViewContent

Sets the deletion action for the dynamic view. You must delete the corresponding item within `action`, as it will be called after the row has already been removed from the List.

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

func onMove(perform: Optional&lt;(IndexSet, Int) -> Void>) -> some DynamicViewContent

Sets the move action for the dynamic view.

func dropDestination&lt;T>(for: T.Type, action: ([T], Int) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

### Deprecated symbols

func onInsert(of: [String], perform: (Int, [NSItemProvider]) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

Deprecated

### Instance Methods

func onInsert(of:perform:)

Sets the insert action for the dynamic view.

## Relationships

### Inherits From

- View

### Conforming Types

- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `View`.

- ModifiedContent

  Conforms when `Content` conforms to `DynamicViewContent` and `Modifier` conforms to `ViewModifier`.

## See Also

### Iterating over dynamic data

struct ForEach

A structure that computes views on demand from an underlying collection of identified data.

struct ForEachSectionCollection

A collection which allows a view to be treated as a collection of its sections in a for each loop.

struct ForEachSubviewCollection

A collection which allows a view to be treated as a collection of its subviews in a for each loop.

