

- Core Foundation
-  CFFileSecurityClearOptions 

Structure

# CFFileSecurityClearOptions

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CFFileSecurityClearOptions
```

## Topics

### Constants

static var accessControlList: CFFileSecurityClearOptions

Clear the access control list.

static var group: CFFileSecurityClearOptions

Clear the (POSIX) group ID.

static var groupUUID: CFFileSecurityClearOptions

Clear the group UUID (for the access control list).

static var mode: CFFileSecurityClearOptions

Clear the file’s mode (POSIX permissions).

static var owner: CFFileSecurityClearOptions

Clear the (POSIX) owner ID.

static var ownerUUID: CFFileSecurityClearOptions

Clear the owner UUID (for the access control list).

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enumerations

struct CFISO8601DateFormatOptions

enum CFRunLoopRunResult

struct CFURLEnumeratorOptions

Options for controlling enumerator behavior.

enum CFURLEnumeratorResult

Result codes from the CFURLEnumeratorGetNextURL(_:_:_:) function.

enum CGRectEdge

