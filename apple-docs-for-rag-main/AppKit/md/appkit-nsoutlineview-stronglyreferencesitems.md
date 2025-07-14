

- AppKit
- NSOutlineView
-  stronglyReferencesItems 

Instance Property

# stronglyReferencesItems

A Boolean value that indicates whether the outline view retains and releases the objects returned from its data source.

macOS 10.12+

``` source
@MainActor
var stronglyReferencesItems: Bool { get set }
```

## Discussion

When the value of this property is true, the outline view retains and releases the objects returned to it from dataSource. When the value is false, the outline view treats the objects as opaque items and assumes that the client has a retain on them. The default value is true for applications linked on macOS 10.12 and later, and false for applications linked on earlier versions of macOS. If you require the legacy behavior and your app links in macOS 10.12 or later, the value of this property must be explicitly set to false in code, because it is not encoded in the nib. In general, this is required if the items themselves create a retain cycle.

## See Also

### Accessing the Data Source

var dataSource: (any NSOutlineViewDataSource)?

The object that provides the data displayed by the receiver.

