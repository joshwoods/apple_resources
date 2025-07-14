

- ManagedApp
-  ManagedAppConfigurationDecodingError 

Protocol

# ManagedAppConfigurationDecodingError

A protocol for an error that describes an issue with decoding the configuration.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
protocol ManagedAppConfigurationDecodingError : Decodable, Encodable, Error
```

## Mentioned in 

Specifying and decoding a configuration

## Overview

For more information, see configurations(_:).

## Topics

### Identifying an error

var code: ManagedAppConfigurationDecodingErrorCode

An app-specific error code that identifies a configuration issue.

**Required**

### Interpreting an error

var message: String

A human-readable message that describes the configuration issue.

**Required**

## Relationships

### Inherits From

- Decodable
- Encodable
- Error
- Sendable

## See Also

### Errors

enum ManagedAppError

Errors that functions in the ManagedApp framework can throw.

struct ManagedAppConfigurationDecodingErrorCode

A code for an error that occurs during configuration decoding.

