

- LightweightCodeRequirements
-  InfoPlistHash 

Structure

# InfoPlistHash

A constraint that tests the specified hash against the Information property list hash stored in the code signature of the process or code file.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct InfoPlistHash
```

## Topics

### Initializers

init(Data)

Match against a single Info.plist hash

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder

### Type Aliases

typealias DataType

typealias OutType

The type of this constraint: InfoPlistHash.

### Type Methods

static func `in`(InfoPlistHash.DataType...) -> InfoPlistHash.OutType

Match against any of the Info.plist hashes in the provided list.

static func `in`([InfoPlistHash.DataType]) -> InfoPlistHash.OutType

Match against any of the Info.plist hashes in the provided list.

## Relationships

### Conforms To

- Decodable
- Encodable
- LaunchConstraint
- OnDiskConstraint
- ProcessConstraint
- Sendable

## See Also

### Testing properties of executable code

struct CodeDirectoryHash

A constraint that matches the hash of a code directory of a code file or of a running or launching process.

class EntitlementsQuery

A constraint that tests values in the entitlements dictionary associated with a process or code file.

struct IsInitProcess

A constraint that tests whether a process is the operating system’s initial process.

struct IsMainBinary

A constraint that tests whether a code file is a main binary.

struct IsSIPProtected

A constraint that tests whether a code file or process is on a volume protected by System Integrity Protection (SIP).

struct PlatformType

A constraint that tests whether a code file or running process targets a given platform.

struct SigningIdentifier

A constraint that tests whether the provided signing identifier matches the signature attached to the code.

struct TeamIdentifier

A constraint that tests whether the provided team identifier matches the team identified in the code signature.

struct ValidationCategory

A constraint that tests whether a code file or running process is signed in a way that conforms to the specified validation category.

