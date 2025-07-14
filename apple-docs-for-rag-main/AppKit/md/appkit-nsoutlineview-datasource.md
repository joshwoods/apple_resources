

- AppKit
- NSOutlineView
-  dataSource 

Instance Property

# dataSource

The object that provides the data displayed by the receiver.

macOS

``` source
@MainActor
weak var dataSource: (any NSOutlineViewDataSource)? { get set }
```

## Discussion

The object must implement the appropriate methods of NSOutlineViewDataSource. See Writing an Outline View Data Source and the NSOutlineViewDataSource Protocol informal protocol specification for more information. Note that in versions of macOS prior to v10.12, the outline view did not retain the data source in a managed memory environment.

Setting the data source invokes tile().

If the data source doesn’t respond to all of the outlineView(_:child:ofItem:), outlineView(_:isItemExpandable:), outlineView(_:numberOfChildrenOfItem:), and outlineView(_:objectValueFor:byItem:) methods, an internalInconsistencyException may be raised.

## See Also

### Related Documentation

Drag and Drop Programming Topics

Outline View Programming Topics

### Accessing the Data Source

var stronglyReferencesItems: Bool

A Boolean value that indicates whether the outline view retains and releases the objects returned from its data source.

