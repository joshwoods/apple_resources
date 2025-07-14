

- Open Directory
-  ODRecord 

Class

# ODRecord

An `ODRecord` object serves as a Cocoa wrapper for an Open Directory record.

Mac CatalystmacOS

``` source
class ODRecord
```

## Topics

### Managing Authentication

func changePassword(String!, toPassword: String!) throws

Changes the record’s password.

func setNodeCredentials(String!, password: String!) throws

Sets credentials for the record’s node.

func setNodeCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyExtended(withAuthenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Verifies the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyPassword(String!) throws

Verifies the password for interaction with the record.

### Managing Group Records

func addMemberRecord(ODRecord!) throws

Adds a member record to this group record.

func isMemberRecord(ODRecord!) throws

Determines whether a given record is a member of this group record.

func removeMemberRecord(ODRecord!) throws

Removes a record as a member of this group record.

### Managing Record Attributes

func addValue(Any!, toAttribute: String!) throws

Adds a value to an attribute of the record.

func recordDetails(forAttributes: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary of attributes with their respective values.

var recordName: String!

The official name of the record.

var recordType: String!

The record’s type.

func removeValues(forAttribute: String!) throws

Removes all values from an attribute of the record.

func removeValue(Any!, fromAttribute: String!) throws

Removes a value from an attribute of the record.

func setValue(Any!, forAttribute: String!) throws

Sets the values of an attribute of the record.

func synchronize() throws

Synchronizes the record from the directory to get current data and commit changes.

func values(forAttribute: String!) throws -> [Any]

Returns the values of an attribute of the record.

### Deleting a Record

func delete() throws

Deletes the record from its node and invalidates it.

### Instance Properties

var secondsUntilAuthenticationsExpire: Int64

var secondsUntilPasswordExpires: Int64

### Instance Methods

func accountPolicies() throws -> [AnyHashable : Any]

func addAccountPolicy([AnyHashable : Any]!, toCategory: String!) throws

func authenticationAllowed() throws

func effectivePolicies() throws -> [AnyHashable : Any]

func passwordChangeAllowed(String!) throws

func policies() throws -> [AnyHashable : Any]

func removeAccountPolicy([AnyHashable : Any]!, fromCategory: String!) throws

func removePolicy(String!) throws

func setAccountPolicies([AnyHashable : Any]!) throws

func setPolicies([AnyHashable : Any]!) throws

func setPolicy(String!, value: Any!) throws

func supportedPolicies() throws -> [AnyHashable : Any]

func willAuthenticationsExpire(UInt64) -> Bool

func willPasswordExpire(UInt64) -> Bool

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

class ODRecordMap

class ODRecordRef

An Open Directory record type.

class ODSession

An `ODSession` object serves as a Cocoa wrapper for an Open Directory session.

class ODSessionRef

An Open Directory session type.

