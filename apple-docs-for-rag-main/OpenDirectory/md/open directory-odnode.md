

- Open Directory
-  ODNode 

Class

# ODNode

An `ODNode` object serves as a Cocoa wrapper for an Open Directory node.

Mac CatalystmacOS

``` source
class ODNode
```

## Topics

### Creating and Initializing a Node

init(session: ODSession!, name: String!) throws

Creates a node object with a specified session and name.

init(session: ODSession!, type: ODNodeType) throws

Creates a node object with a specified session and type.

### Querying a Node

func customCall(Int, send: Data!) throws -> Data

Returns the result of a custom call to the node.

func nodeDetails(forKeys: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary containing details about a node.

var nodeName: String!

The node’s name.

func subnodeNames() throws -> [Any]

Returns the names of subnodes for the node.

func unreachableSubnodeNames() throws -> [Any]

Returns an array of the subnodes of a given node that are currently unreachable.

### Setting Node Credentials

func setCredentialsWithRecordType(String!, recordName: String!, password: String!) throws

Sets credentials for interacting with the node.

func setCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the node using other types of authentication available to Open Directory.

func setCredentialsUsingKerberosCache(String!) throws

Sets the credentials for interaction with the node using a Kerberos cache.

### Managing Node Records

func createRecord(withRecordType: String!, name: String!, attributes: [AnyHashable : Any]!) throws -> ODRecord

Creates a record in a specified node with specified properties.

func record(withRecordType: String!, name: String!, attributes: Any!) throws -> ODRecord

Returns a record from the node with a specified type and name.

func supportedAttributes(forRecordType: String!) throws -> [Any]

Returns an array of attribute types supported by the node’s records.

func supportedRecordTypes() throws -> [Any]

Returns an array of the record types supported by the node.

### Instance Properties

var configuration: ODConfiguration!

### Instance Methods

func accountPolicies() throws -> [AnyHashable : Any]

func addAccountPolicy([AnyHashable : Any]!, toCategory: String!) throws

func customFunction(String!, payload: Any!) throws -> Any

func passwordContentCheck(String!, forRecordName: String!) throws

func policies() throws -> [AnyHashable : Any]

func removeAccountPolicy([AnyHashable : Any]!, fromCategory: String!) throws

func removePolicy(String!) throws

func setAccountPolicies([AnyHashable : Any]!) throws

func setPolicies([AnyHashable : Any]!) throws

func setPolicy(String!, value: Any!) throws

func supportedPolicies() throws -> [AnyHashable : Any]

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

