

- iAd
-  ADClientError Deprecated

Structure

# ADClientError

The group of error codes that pass from the attribution response to the completion handler block.

``` source
struct ADClientError
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Mentioned in 

iAd Changelog

## Overview

When you call the requestAttributionDetails(_:) method, error codes are passed from the attribution response to the completion handler block.

## Topics

### Error Codes

static var corruptResponse: ADClientError.Code

The response received from the attribution server was corrupt.

static var requestClientError: ADClientError.Code

The response received from the attribution server had an HTTP 4xx status code.

static var requestNetworkError: ADClientError.Code

The communication with the attribution server had a network error.

static var requestServerError: ADClientError.Code

The response received from the attribution server had an HTTP 5xx status code.

static var trackingRestrictedOrDenied: ADClientError.Code

The user is restricted or has denied tracking for the calling application.

static var missingData: ADClientError.Code

The downloaded app received a payload lacking enough data to perform an attribution check.

static var unsupportedPlatform: ADClientError.Code

The attribution API was called on an unsupported platform.

static var limitAdTracking: ADClientError.Code

static var unknown: ADClientError.Code

enum Code

The error codes that pass from the attribution response to the completion handler.

### Error Characteristics

let ADClientErrorDomain: String

The error domain that passes to the completion handler.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Attribution Errors

let ADClientErrorDomain: String

The error domain that passes to the completion handler.

Deprecated

enum Code

The error codes that pass from the attribution response to the completion handler.

Deprecated

