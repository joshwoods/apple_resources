

- Open Directory
-  ODQuery 

Class

# ODQuery

An `ODQuery` object serves as a Cocoa wrapper for an Open Directory query.

Mac CatalystmacOS

``` source
class ODQuery
```

## Topics

### Creating and Initializing a Query

init(node: ODNode!, forRecordTypes: Any!, attribute: String!, matchType: ODMatchType, queryValues: Any!, returnAttributes: Any!, maximumResults: Int) throws

Creates a query object with provided parameters.

### Managing Asynchronous Queries

var delegate: (any ODQueryDelegate)!

The query’s delegate.

var operationQueue: OperationQueue!

The queue on which asynchronous results are delivered to the delegate.

func schedule(in: RunLoop!, forMode: String!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func remove(from: RunLoop!, forMode: String!)

Removes the query from a specified run loop.

func synchronize()

Restarts a query, disposing of any results it has obtained.

### Managing Synchronous Queries

func resultsAllowingPartial(Bool) throws -> [Any]

Returns results from a query synchronously.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

