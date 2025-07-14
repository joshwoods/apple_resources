

- BrowserEngineKit
-  RestrictedSandboxRevision 

Enumeration

# RestrictedSandboxRevision

Revisions to the restricted sandbox rules.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
enum RestrictedSandboxRevision
```

## Overview

Design your browser to support the latest revision to the restricted sandbox in all extensions, and opt in to new revisions as they become available.

## Topics

### Sandbox restriction revisions

case revision1

Revision 1 of the restricted sandbox rules.

### Operators

static func == (RestrictedSandboxRevision, RestrictedSandboxRevision) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (RestrictedSandboxRevision, RestrictedSandboxRevision) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [RestrictedSandboxRevision]

A collection of all values of this type.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Comparable
- Copyable
- Equatable
- Hashable

## See Also

### Access control

Limiting resource access in web content extensions

Reduce the impact of vulnerabilities in web content extensions by limiting privileges.

Accessing files in browser extensions

Grant extensions access to files from within your browser app.

Attributing memory to a content extension

Adhere to operating-system limits on GPU memory use.

protocol RestrictedSandboxAppliable

A protocol that browser extensions implement to opt into a more restricted sandbox.

