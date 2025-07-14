

- AppKit
- NSTreeController
-  sortDescriptors 

Instance Property

# sortDescriptors

An array containing the sort descriptors used to arrange the tree controller’s content.

macOS

``` source
var sortDescriptors: [NSSortDescriptor] { get set }
```

## Discussion

When the value of this property is an empty array, the tree controller has no sort descriptors configured, which means that the contents are arranged in their natural order. This property is observable using key-value observing.

## See Also

### Related Documentation

Cocoa Bindings Programming Topics

