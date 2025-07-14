

- ManagedSettings
-  Application 

Structure

# Application

A representation of an application on the user’s device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct Application
```

## Overview

Managed Settings represents apps with tokens to preserve user privacy and control.

## Topics

### Creating an Application

init(bundleIdentifier: String)

Creates an object that represents the app with the specified bundle identifier.

init(token: ApplicationToken)

Creates an object that represents the app with the specified token.

### Accessing Application Information

let bundleIdentifier: String?

The unique string that identifies this app.

let token: ApplicationToken?

An opaque representation of a specific web domain.

let localizedDisplayName: String?

A localized display name for the application.

### Comparing Applications

static func == (Application, Application) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Apps

typealias ApplicationToken

A representation of an application.

