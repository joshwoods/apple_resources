

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  MobileDriversLicenseDisplayRequest.Options 

Structure

# MobileDriversLicenseDisplayRequest.Options

An object that customizes how to perform a display request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Options
```

## Overview

Use this object to configure the validation mode of the request.

## Topics

### Structures

struct ValidationMode

A type that represents the validation mode of the mobile document request.

### Operators

static func == (MobileDriversLicenseDisplayRequest.Options, MobileDriversLicenseDisplayRequest.Options) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(validationMode: MobileDriversLicenseDisplayRequest.Options.ValidationMode)

Creates a mobile document reader display request options type.

### Instance Properties

var hashValue: Int

The hash value.

var validationMode: MobileDriversLicenseDisplayRequest.Options.ValidationMode

The validation mode of the mobile document request.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring a display request

var options: MobileDriversLicenseDisplayRequest.Options

An object that customizes how to perform a display request.

