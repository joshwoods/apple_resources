

- MarketplaceKit
- AppLibrary
-  AppLibrary.App 

Class

# AppLibrary.App

Information about an app that someone installs from a marketplace, including its ID and installation status.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
final class App
```

## Topics

### Structures

struct Installation

struct Metadata

### Operators

static func == (AppLibrary.App, AppLibrary.App) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let id: AppleItemID

The stable identity of the entity associated with this instance.

var installation: AppLibrary.App.Installation?

var installationError: MarketplaceKitError?

An error that occurs during the installation of an app that resides on a marketplace.

var installedMetadata: AppLibrary.App.Metadata?

var isInstalled: Bool

var isInstalling: Bool

var isUpdating: Bool

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable
- Observable
- Sendable

