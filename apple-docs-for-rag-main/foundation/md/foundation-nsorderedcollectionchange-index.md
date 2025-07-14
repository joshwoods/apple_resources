

- Foundation
- NSOrderedCollectionChange
-  index 

Instance Property

# index

The index location of the change.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var index: Int { get }
```

## See Also

### Accessing the Change

var changeType: NSCollectionChangeType

The type of change.

var object: Any?

An object the change inserts or removes.

var associatedIndex: Int

When this property is set to a value other than NSNotFound, the receiver is one half of a move, and this value is the index of the change’s counterpart of the opposite type in the diff.

