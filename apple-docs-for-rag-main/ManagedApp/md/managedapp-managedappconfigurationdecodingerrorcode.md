

- ManagedApp
-  ManagedAppConfigurationDecodingErrorCode 

Structure

# ManagedAppConfigurationDecodingErrorCode

A code for an error that occurs during configuration decoding.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
struct ManagedAppConfigurationDecodingErrorCode
```

## Mentioned in 

Specifying and decoding a configuration

## Overview

The system reserves some codes for its use only. Reserved codes are equal to or greater than `firstReserved`. Codes less than the `firstReserved` value are app-specific. For more information, see code.

## Topics

### Initializing an error

init?(rawValue: Int)

Initializes a configuration decoding error code.

### Identifying an error

let rawValue: Int

The error code’s value in its underlying type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let dataCorrupted: Int

An error code that indicates the decoder encountered corrupt data.

static let firstReserved: Int

An error code for the start of the range of reserved error codes.

static let generic: Int

A reserved error that indicates the decoder threw an unknown custom error.

static let keyNotFound: Int

An error code that indicates the decoder encountered an unknown coding key.

static let timeout: Int

An error code that indicates the decoder timed out.

static let typeMismatch: Int

An error code that indicates the decoder encountered a type mismatch.

static let valueNotFound: Int

An error code that indicates a coding key yields no value.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

enum ManagedAppError

Errors that functions in the ManagedApp framework can throw.

protocol ManagedAppConfigurationDecodingError

A protocol for an error that describes an issue with decoding the configuration.

