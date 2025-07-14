

- Core Data
- NSPropertyDescription
-  name 

Instance Property

# name

The name of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var name: String { get set }
```

## Discussion

A property name cannot be the same as any no-parameter method name of `NSObject` or `NSManagedObject`. Since there are hundreds of methods on `NSObject` which may conflict with property names, you should avoid very general words (like “font”, and “color”) and words or phrases that overlap with Cocoa paradigms (such as “isEditing” and “objectSpecifier”).

### Special Considerations

Setting the name raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

