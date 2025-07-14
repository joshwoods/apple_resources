

- Open Directory
-  ODConfiguration 

Class

# ODConfiguration

Mac CatalystmacOS 10.9+

``` source
class ODConfiguration
```

## Topics

### Instance Properties

var authenticationModuleEntries: [Any]!

var comment: String!

var connectionIdleTimeoutInSeconds: Int

var connectionSetupTimeoutInSeconds: Int

var defaultMappings: ODMappings!

var defaultModuleEntries: [Any]!

var discoveryModuleEntries: [Any]!

var generalModuleEntries: [Any]!

var hideRegistration: Bool

var manInTheMiddleProtection: Bool

var nodeName: String!

var packetEncryption: Int

var packetSigning: Int

var preferredDestinationHostName: String!

var preferredDestinationHostPort: UInt16

var queryTimeoutInSeconds: Int

var templateName: String!

var trustAccount: String!

var trustKerberosPrincipal: String!

var trustMetaAccount: String!

var trustType: String!

var trustUsesKerberosKeytab: Bool

var trustUsesMutualAuthentication: Bool

var trustUsesSystemKeychain: Bool

var virtualSubnodes: [Any]!

### Instance Methods

func addTrustType(String!, trustAccount: String!, trustPassword: String!, username: String!, password: String!, joinExisting: Bool) throws

func removeTrust(usingUsername: String!, password: String!, deleteTrustAccount: Bool) throws

func save(using: SFAuthorization!) throws

### Type Methods

class func suggestedTrustAccount(String!) -> String!

class func suggestedTrustPassword(Int) -> String!

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

class ODSession

An `ODSession` object serves as a Cocoa wrapper for an Open Directory session.

class ODSessionRef

An Open Directory session type.

