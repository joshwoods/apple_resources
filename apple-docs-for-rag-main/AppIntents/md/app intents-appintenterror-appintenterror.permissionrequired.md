

- App Intents
- AppIntentError
-  AppIntentError.PermissionRequired 

Enumeration

# AppIntentError.PermissionRequired

Errors that indicate that the app doesn’t have required permission to perform an action

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum PermissionRequired
```

## Overview

Use the permission errors to inform a person that the app requires specific permissions and that they need to grant a permission to successfully complete the action.

## Topics

### Type Properties

static let bluetooth: AppIntentError

User needs to grant bluetooth permission to the app

static let contacts: AppIntentError

User needs to grant contacts permission to the app

static let localNetwork: AppIntentError

User needs to grant local network access to the app

static let photos: AppIntentError

User needs to grant photos permission to the app

static let siri: AppIntentError

User needs to grant Siri permission to the app

### Type Methods

static func location(precise: Bool) -> AppIntentError

User needs to grant location permission to the app.

