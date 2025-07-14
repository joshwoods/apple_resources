

- App Intents
- AppIntentError
-  AppIntentError.UserActionRequired 

Enumeration

# AppIntentError.UserActionRequired

Errors that represent a state where a person needs to do respond in order to successfully completed successfully the action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum UserActionRequired
```

## Overview

Use the system-defined errors to inform a person about steps they can take to fix the error.

## Topics

### Type Properties

static let accountSetup: AppIntentError

User needs to setup their account

static let confirmation: AppIntentError

User needs to confirm the action

static let signin: AppIntentError

User needs to sign in to continue

