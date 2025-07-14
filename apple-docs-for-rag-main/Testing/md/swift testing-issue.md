

- Swift Testing
-  Issue 

Structure

# Issue

A type describing a failure or warning which occurred during a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Issue
```

## Mentioned in 

Interpreting bug identifiers

Associating bugs with tests

## Topics

### Instance Properties

var comments: [Comment]

Any comments provided by the developer and associated with this issue.

var error: (any Error)?

The error which was associated with this issue, if any.

var kind: Issue.Kind

The kind of issue this value represents.

var sourceLocation: SourceLocation?

The location in source where this issue occurred, if available.

### Type Methods

static func record(any Error, Comment?, sourceLocation: SourceLocation) -> Issue

Record a new issue when a running test unexpectedly catches an error.

static func record(Comment?, sourceLocation: SourceLocation) -> Issue

Record an issue when a running test fails unexpectedly.

### Enumerations

enum Kind

Kinds of issues which may be recorded.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Sendable

