

- ClassKit
-  CLSObject 

Class

# CLSObject

The abstract base class for objects managed by ClassKit.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
class CLSObject
```

## Topics

### Accessing Object Information

var dateCreated: Date

The date on which the object was created.

var dateLastModified: Date

The date on which the object was last modified.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLSActivity
- CLSActivityItem
- CLSContext
- CLSProgressReportingCapability

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating contexts

init(type: CLSContextType, identifier: String, title: String)

Initializes a new context.

