

- ManagedSettings
- ManagedSettingsStore
-  ManagedSettingsStore.Name 

Structure

# ManagedSettingsStore.Name

The unique name of a store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Name
```

## Overview

Use `ManagedSettingsStore.Name` to create distinct stores with their own settings. Initializing multiple stores with the same name will share settings.

## Topics

### Initializers

init(String)

Creates a new instance with the specified string.

init(rawValue: String)

Creates a new instance with the specified string.

### Instance Properties

let rawValue: String

The name of the store as a `String`.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let `default`: ManagedSettingsStore.Name

The default store name.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

