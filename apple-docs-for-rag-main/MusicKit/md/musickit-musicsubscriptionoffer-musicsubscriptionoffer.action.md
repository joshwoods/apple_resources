

- MusicKit
- MusicSubscriptionOffer
-  MusicSubscriptionOffer.Action 

Structure

# MusicSubscriptionOffer.Action

A representation of the entry point for the sheet with subscription offers for Apple Music.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Action
```

## Topics

### Initializers

init(String)

Creates an action with the specified raw value.

init(rawValue: String)

Creates an action with the specified raw value.

### Instance Properties

let rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let subscribe: MusicSubscriptionOffer.Action

An action for inviting the user to subscribe to Apple Music.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

