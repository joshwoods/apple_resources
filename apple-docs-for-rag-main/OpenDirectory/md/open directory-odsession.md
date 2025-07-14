

- Open Directory
-  ODSession 

Class

# ODSession

An `ODSession` object serves as a Cocoa wrapper for an Open Directory session.

Mac CatalystmacOS

``` source
class ODSession
```

## Topics

### Creating and Accessing Sessions

class func `default`() -> ODSession!

Returns a shared instance of the local session.

init(options: [AnyHashable : Any]!) throws

Creates a session object directed over proxy to another host.

### Accessing Node Information

func nodeNames() throws -> [Any]

Returns the node names that are registered with this session.

### Constants

ODSession Option Keys

Option keys used when creating a session directed over a proxy.

### Instance Properties

var configurationTemplateNames: [Any]!

var mappingTemplateNames: [Any]!

### Instance Methods

func add(ODConfiguration!, authorization: SFAuthorization!) throws

func configuration(forNodename: String!) -> ODConfiguration!

func configurationAuthorizationAllowingUserInteraction(Bool) throws -> SFAuthorization

func delete(ODConfiguration!, authorization: SFAuthorization!) throws

func deleteConfiguration(withNodename: String!, authorization: SFAuthorization!) throws

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

class ODModuleEntry

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

class ODSessionRef

An Open Directory session type.

