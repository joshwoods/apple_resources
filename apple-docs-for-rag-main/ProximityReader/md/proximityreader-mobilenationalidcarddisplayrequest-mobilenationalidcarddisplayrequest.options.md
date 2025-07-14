

- ProximityReader
- MobileNationalIDCardDisplayRequest
-  MobileNationalIDCardDisplayRequest.Options 

Structure

# MobileNationalIDCardDisplayRequest.Options

An object that customizes how to perform a display request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

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

static func == (MobileNationalIDCardDisplayRequest.Options, MobileNationalIDCardDisplayRequest.Options) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(validationMode: MobileNationalIDCardDisplayRequest.Options.ValidationMode)

Creates a mobile document reader display request options type.

### Instance Properties

var hashValue: Int

The hash value.

var validationMode: MobileNationalIDCardDisplayRequest.Options.ValidationMode

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

### Configuring the request details

var region: Locale.Region

The region of the document you’re requesting.

var elements: [MobileNationalIDCardDisplayRequest.Element]

The document elements you’re requesting.

struct Element

A type that represents an element you can request from a mobile national ID card.

var options: MobileNationalIDCardDisplayRequest.Options

An object that customizes how to perform a display request.

