

- ProximityReader
- MobileNationalIDCardDisplayRequest
- MobileNationalIDCardDisplayRequest.Options
-  MobileNationalIDCardDisplayRequest.Options.ValidationMode 

Structure

# MobileNationalIDCardDisplayRequest.Options.ValidationMode

A type that represents the validation mode of the mobile document request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct ValidationMode
```

## Overview

The validation mode controls how the system UI behaves when a display request has been successfully performed.

## Topics

### Operators

static func == (MobileNationalIDCardDisplayRequest.Options.ValidationMode, MobileNationalIDCardDisplayRequest.Options.ValidationMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let check: MobileNationalIDCardDisplayRequest.Options.ValidationMode

A button that enables the user to perform a single document request.

static let checkMultiple: MobileNationalIDCardDisplayRequest.Options.ValidationMode

A button that enables the user to perform multiple document requests in one session.

static let confirm: MobileNationalIDCardDisplayRequest.Options.ValidationMode

Confirmation buttons that enable the user to express their validation decision.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

