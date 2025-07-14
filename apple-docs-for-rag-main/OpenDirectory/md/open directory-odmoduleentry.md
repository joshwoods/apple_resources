

- Open Directory
-  ODModuleEntry 

Class

# ODModuleEntry

Mac CatalystmacOS 10.9+

``` source
class ODModuleEntry
```

## Topics

### Initializers

convenience init!(name: String!, xpcServiceName: String!)

### Instance Properties

var mappings: ODMappings!

var name: String!

var supportedOptions: [Any]!

var uuidString: String!

var xpcServiceName: String!

### Instance Methods

func option(String!) -> Any!

func setOption(String!, value: Any!)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class ODAttributeMap

class ODConfiguration

class ODContext

An Open Directory context type.

class ODMappings

class ODNode

An `ODNode` object serves as a Cocoa wrapper for an Open Directory node.

class ODNodeRef

An Open Directory node type.

class ODQuery

An `ODQuery` object serves as a Cocoa wrapper for an Open Directory query.

class ODQueryRef

An Open Directory query type.

class ODRecord

An `ODRecord` object serves as a Cocoa wrapper for an Open Directory record.

class ODRecordMap

class ODRecordRef

An Open Directory record type.

class ODSession

An `ODSession` object serves as a Cocoa wrapper for an Open Directory session.

class ODSessionRef

An Open Directory session type.

