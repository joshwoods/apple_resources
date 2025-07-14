

- ProximityReader
- MobileDriversLicenseDisplayRequest
- MobileDriversLicenseDisplayRequest.Options
-  MobileDriversLicenseDisplayRequest.Options.ValidationMode 

Structure

# MobileDriversLicenseDisplayRequest.Options.ValidationMode

A type that represents the validation mode of the mobile document request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct ValidationMode
```

## Overview

The validation mode controls how the system UI behaves when a display request has been successfully performed.

## Topics

### Operators

static func == (MobileDriversLicenseDisplayRequest.Options.ValidationMode, MobileDriversLicenseDisplayRequest.Options.ValidationMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let check: MobileDriversLicenseDisplayRequest.Options.ValidationMode

A button that enables the user to perform a single document request.

static let checkMultiple: MobileDriversLicenseDisplayRequest.Options.ValidationMode

A button that enables the user to perform multiple document requests in one session.

static let confirm: MobileDriversLicenseDisplayRequest.Options.ValidationMode

Confirmation buttons that enable the user to express their validation decision.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

