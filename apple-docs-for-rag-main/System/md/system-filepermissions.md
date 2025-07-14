

- System
-  FilePermissions 

Structure

# FilePermissions

The access permissions for a file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct FilePermissions
```

## Overview

The following example creates an instance of the `FilePermissions` structure from a raw octal literal and compares it to a file permission created using named options:

```
let perms = FilePermissions(rawValue: 0o644)
perms == [.ownerReadWrite, .groupRead, .otherRead] // true
```

## Topics

### Owner Permissions

static var ownerRead: FilePermissions

Indicates that the owner has read-only permission.

static var ownerWrite: FilePermissions

Indicates that the owner has write-only permission.

static var ownerExecute: FilePermissions

Indicates that the owner has execute-only permission.

static var ownerReadWrite: FilePermissions

Indicates that the owner has read-write permission.

static var ownerReadExecute: FilePermissions

Indicates that the owner has read-execute permission.

static var ownerWriteExecute: FilePermissions

Indicates that the owner has write-execute permission.

static var ownerReadWriteExecute: FilePermissions

Indicates that the owner has read, write, and execute permission.

### Group Permissions

static var groupRead: FilePermissions

Indicates that the group has read-only permission.

static var groupWrite: FilePermissions

Indicates that the group has write-only permission.

static var groupExecute: FilePermissions

Indicates that the group has execute-only permission.

static var groupReadWrite: FilePermissions

Indicates that the group has read-write permission.

static var groupReadExecute: FilePermissions

Indicates that the group has read-execute permission.

static var groupWriteExecute: FilePermissions

Indicates that the group has write-execute permission.

static var groupReadWriteExecute: FilePermissions

Indicates that the group has read, write, and execute permission.

### Other Permissions

static var otherRead: FilePermissions

Indicates that other users have read-only permission.

static var otherWrite: FilePermissions

Indicates that other users have write-only permission.

static var otherExecute: FilePermissions

Indicates that other users have execute-only permission.

static var otherReadWrite: FilePermissions

Indicates that other users have read-write permission.

static var otherReadExecute: FilePermissions

Indicates that other users have read-execute permission.

static var otherWriteExecute: FilePermissions

Indicates that other users have write-execute permission.

static var otherReadWriteExecute: FilePermissions

Indicates that other users have read, write, and execute permission.

### Special Permissions

static var setUserID: FilePermissions

Indicates that the file is executed as the owner.

static var setGroupID: FilePermissions

Indicates that the file is executed as the group.

static var saveText: FilePermissions

Indicates that executable’s text segment should be kept in swap space even after it exits.

### Interacting with C APIs

init(rawValue: CModeT)

Create a strongly-typed file permission from a raw C value.

let rawValue: CModeT

The raw C file permissions.

typealias CModeT

The C `mode_t` type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Debugging

var description: String

A textual representation of the file permissions.

var debugDescription: String

A textual representation of the file permissions, suitable for debugging.

### Comparing File Permissions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

var hashValue: Int

### Encoding File Permissions

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `UInt16`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `UInt16`.

### Performing Set Operations

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Files

struct FileDescriptor

An abstract handle to an input or output data resource, such as a file or a socket.

struct FilePath

Represents a location in the file system.

