

- LightweightCodeRequirements
-  CodeDirectoryHash 

Structure

# CodeDirectoryHash

A constraint that matches the hash of a code directory of a code file or of a running or launching process.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct CodeDirectoryHash
```

## Overview

In the context of ProcessCodeRequirement and LaunchCodeRequirement this constraint matches the hash of the chosen code directory for the running process, or the process the system is launching.

In the context of OnDiskCodeRequirement this constraint matches the hash of the code directory for the specified `SecStaticCodeRef` that best matches the current architecture. The best match is different for processes running on Intel and Apple silicon, including an Intel process running on Apple silicon with Rosetta. To reliably identify a code file using its code directory hash, use in(_:) and supply a list of the known code directory hash values.

## Topics

### Initializers

init(Data)

Match against a single code directory hash.

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder

### Type Aliases

typealias DataType

The basic input data type for this constraint: Data

typealias OutType

The type of this constraint: CodeDirectoryHash

### Type Methods

static func `in`([CodeDirectoryHash.DataType]) -> CodeDirectoryHash.OutType

Match against any of the code directory hashes in the provided list.

static func `in`(CodeDirectoryHash.DataType...) -> CodeDirectoryHash.OutType

Match against any of the code directory hashes in the provided list.

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

class EntitlementsQuery

A constraint that tests values in the entitlements dictionary associated with a process or code file.

struct InfoPlistHash

A constraint that tests the specified hash against the Information property list hash stored in the code signature of the process or code file.

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

