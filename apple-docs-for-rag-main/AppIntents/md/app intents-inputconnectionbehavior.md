

- App Intents
-  InputConnectionBehavior 

Enumeration

# InputConnectionBehavior

Describes the input behaviors for connecting a parameter to the output of the previous App Intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum InputConnectionBehavior
```

## Topics

### Getting the connection behaviors

case `default`

A behavior that allows the system to determine if the parameter accepts the output.

case never

A behavior that prohibits the parameter from accepting the output.

case connectToPreviousIntentResult

A behavior that permits the parameter to accept the output.

### Operators

static func == (InputConnectionBehavior, InputConnectionBehavior) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Intent parameters

class IntentParameter

A property wrapper that indicates the associated property is an input argument of the app intent.

class IntentParameterDependency

A property wrapper that represents an app intent dependency you use to provide dynamic options.

struct IntentParameterContext

A type that provides information about an associated parameter during value resolution.

