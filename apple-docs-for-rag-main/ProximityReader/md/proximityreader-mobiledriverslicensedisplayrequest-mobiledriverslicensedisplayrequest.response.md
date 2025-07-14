

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  MobileDriversLicenseDisplayRequest.Response 

Structure

# MobileDriversLicenseDisplayRequest.Response

A type that contains the response information from a successful mobile driver’s license display request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Response
```

## Overview

Use this object to check the validation outcome of the display request.

## Topics

### Operators

static func == (MobileDriversLicenseDisplayRequest.Response, MobileDriversLicenseDisplayRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let validationOutcome: MobileDriversLicenseDisplayRequest.Response.ValidationOutcome

The value that indicates how the user validated the mobile document response.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum ValidationOutcome

A type that represents how the user validates the mobile document response.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

