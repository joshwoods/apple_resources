

- ProximityReader
- MobileDocumentReader
-  MobileDocumentReader.Configuration 

Structure

# MobileDocumentReader.Configuration

A type that represents the configuration of the mobile document reader.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Configuration
```

## Overview

Use the reader’s configuration to generate a reader token on your server.

## Topics

### Operators

static func == (MobileDocumentReader.Configuration, MobileDocumentReader.Configuration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let readerInstanceIdentifier: String

The unique identifier for the mobile document reader instance.

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

### Retrieving the reader configuration

var configuration: MobileDocumentReader.Configuration

The configuration of the mobile document reader.

