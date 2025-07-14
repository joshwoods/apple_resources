

- ProximityReader
- MobileNationalIDCardDisplayRequest
-  MobileNationalIDCardDisplayRequest.Response 

Structure

# MobileNationalIDCardDisplayRequest.Response

A type that contains the response information from a successful mobile national ID card display request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Response
```

## Overview

Use this object to check the validation outcome of the display request.

## Topics

### Operators

static func == (MobileNationalIDCardDisplayRequest.Response, MobileNationalIDCardDisplayRequest.Response) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let validationOutcome: MobileNationalIDCardDisplayRequest.Response.ValidationOutcome

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

