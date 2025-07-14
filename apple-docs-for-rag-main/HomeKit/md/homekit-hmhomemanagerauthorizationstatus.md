

- HomeKit
-  HMHomeManagerAuthorizationStatus 

Structure

# HMHomeManagerAuthorizationStatus

The possible home-access states.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct HMHomeManagerAuthorizationStatus
```

## Overview

Inspect the home manager’s authorizationStatus property for one or more of the bits defined by HMHomeManagerAuthorizationStatus.

## Topics

### Recognizing Status Values

static var determined: HMHomeManagerAuthorizationStatus

The user has set the app’s level of access to home data.

static var authorized: HMHomeManagerAuthorizationStatus

The app has access to home data.

static var restricted: HMHomeManagerAuthorizationStatus

The app doesn’t have access to home data.

### Creating an Authorization Status

init(rawValue: UInt)

Creates an access status from a raw value.

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

### Inspecting authorization status

var authorizationStatus: HMHomeManagerAuthorizationStatus

The current state of the app’s access to home data.

