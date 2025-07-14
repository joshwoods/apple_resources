

- App Intents
- AppIntentError
-  AppIntentError.Unrecoverable 

Enumeration

# AppIntentError.Unrecoverable

Unknown or unrecoverable error that might have occurred due to either a system or user error.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Unrecoverable
```

## Overview

Use these system-defined errors to inform a person that there is no immediate way to remedy an error.

## Topics

### Type Properties

static let entityNotFound: AppIntentError

You are looking to fetch an entity that does not exist

static let featureCurrentlyRestricted: AppIntentError

This feature is currently restricted (due to screen time restrictions, MDM profiles etc.)

static let networkFailure: AppIntentError

User needs to be connected to internet

static let notAllowed: AppIntentError

This current action is not allowed

static let partialFailure: AppIntentError

Not every action was completed

static let unknown: AppIntentError

Something went wrong

static let unsupportedOnDevice: AppIntentError

This feature is not supported on this device

