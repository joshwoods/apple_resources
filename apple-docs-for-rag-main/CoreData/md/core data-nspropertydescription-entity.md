

- Core Data
- NSPropertyDescription
-  entity 

Instance Property

# entity

The entity description of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var entity: NSEntityDescription { get }
```

## See Also

### Related Documentation

Core Data Programming Guide

var properties: [NSPropertyDescription]

An array containing the properties of the receiver.

### Accessing Features of a Property

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var name: String

The name of the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

