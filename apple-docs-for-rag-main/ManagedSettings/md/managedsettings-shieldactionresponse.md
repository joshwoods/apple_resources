

- ManagedSettings
-  ShieldActionResponse 

Enumeration

# ShieldActionResponse

Constants your extension that handles shield actions can use to tell the system how to respond to an action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum ShieldActionResponse
```

## Topics

### Responses

case close

An instruction for the system to close the current application or web browser.

case `defer`

An instruction to defer a response to the action.

case none

An instruction that the system doesn’t need to take any additional action on behalf of the extension.

### Comparisons

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Handling Shield Actions

enum ShieldAction

Constants that describe a user’s action for your extension to handle.

