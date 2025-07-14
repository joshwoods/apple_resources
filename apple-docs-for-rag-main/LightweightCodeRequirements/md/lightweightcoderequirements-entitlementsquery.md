

- LightweightCodeRequirements
-  EntitlementsQuery 

Class

# EntitlementsQuery

A constraint that tests values in the entitlements dictionary associated with a process or code file.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
class EntitlementsQuery
```

## Overview

Entitlements dictionaries use strings for keys. The value of each key could be a bool, integer, string, array or another dictionary. Arrays are homogenous. Entitlements queries are a chain of operations that allow matching against arbitrarily nested values in the dictionary.

Example entitlements dictionary:

```
```

Example query to match the first entitlement exactly

```
```

Example query to match the second entitlement exactly.

```
```

or to match the second entitlement less specifically

```
```

The following query will detect the presence of the com.apple.private.hid.client.event-dispatch.internal key without checking its value.

```
```

To match its value add a match() call to the chain.

```
```

The following example demonstrate the keyPrefix query.

```
```

The keyPrefix query will match the “com.apple.application-identifier” only. Then the match query will fail because true does not match “com.apple.TextEdit”.

This constraint will cause a matching failure if the process or file being matched does not include entitlements.

## Topics

### Initializers

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func elementAtIndex(Int64) -> EntitlementsQuery

Match against the specified index (0 based) in an array. Chain additional qualifiers to constrain the value of element.

func encode(to: any Encoder) throws

Encodes this value into the given encoder

func key(String) -> EntitlementsQuery

Match the specified key in a nested dictionary

func keyPrefix(String) -> EntitlementsQuery

Match the specified key prefix in a nested dictionary.

func match(String) -> EntitlementsQuery

Match the specified string value against a string or an array of strings.

func match(Bool) -> EntitlementsQuery

Match the specified bool value against a bool value.

func match(Int64) -> EntitlementsQuery

Match the specified Int64 against an integer or array of integers.

func matchPrefix(String) -> EntitlementsQuery

Match the specified string prefix against a string value or array.

func matchPrefixSingle(String) -> EntitlementsQuery

Match the specified string prefix value against a string value (not an array).

func matchSingle(Int64) -> EntitlementsQuery

Match the specified Int64 value against an integer value (not an array).

func matchSingle(String) -> EntitlementsQuery

Match the specified string against a string value (not an array).

func matchType(EntitlementsQuery.DataType) -> EntitlementsQuery

Matches the specified type against the current element.

### Type Methods

static func key(String) -> EntitlementsQuery

Match against the specified key name at the root of the entitlements dictionary.

static func keyPrefix(String) -> EntitlementsQuery

Match the specified key prefix at the root of the entitlements dicitonary. Chain additional qualifiers to constrain the value of the key.

### Enumerations

enum DataType

The types of elements allowed in entitlements dictionaries.

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

