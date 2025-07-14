

- Core Location
- CLError
-  CLError.Code 

Enumeration

# CLError.Code

Error codes returned by the location manager object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Code
```

## Overview

Instances of NSError object delivered to the delegate use these error codes for the code property of the error object.

## Topics

### Getting general errors

case locationUnknown

A constant that indicates the location manager was unable to obtain a location value right now.

case denied

A constant that indicates the user denied access to the location service.

case promptDeclined

A constant that indicates the user didn’t grant the requested temporary authorization.

case network

A constant that indicates the network was unavailable or a network error occurred.

case headingFailure

A constant that indicates the location manager can’t determine the heading.

case rangingUnavailable

A constant that indicates ranging is disabled.

case rangingFailure

A constant that indicates a general ranging error occurred.

### Getting region monitoring errors

case regionMonitoringDenied

A constant that indicates the user denied access to the region monitoring service.

case regionMonitoringFailure

A constant that indicates the location manager failed to monitor a registered region.

case regionMonitoringSetupDelayed

A constant that indicates Core Location failed to initialize the region monitoring feature.

case regionMonitoringResponseDelayed

A constant that indicates Core Location will deliver events but they may be delayed.

### Getting geocoding errors

case geocodeCanceled

A constant that indicates the geocode request was canceled.

case geocodeFoundNoResult

A constant that indicates the geocode request yielded no result.

case geocodeFoundPartialResult

A constant that indicates the geocode request yielded a partial result.

### Getting deferred location update errors

case deferredFailed

A constant that indicates the location manager didn’t enter deferred mode for an unknown reason.

case deferredCanceled

A constant that indicates your app or the location manager canceled the request for deferred updates.

case deferredAccuracyTooLow

A constant that indicates deferred mode isn’t supported for the requested accuracy.

case deferredDistanceFiltered

A constant that indicates deferred mode doesn’t support distance filters.

case deferredNotUpdatingLocation

A constant that indicates the location manager didn’t enter deferred mode because location updates were already disabled or paused.

### Enumeration cases

case historicalLocationError

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting general errors

static var locationUnknown: CLError.Code

A constant that indicates the location manager was unable to obtain a location value right now.

static var denied: CLError.Code

A constant that indicates the user denied access to the location service.

static var promptDeclined: CLError.Code

A constant that indicates the user didn’t grant the requested temporary authorization.

static var network: CLError.Code

A constant that indicates the network was unavailable or a network error occurred.

static var headingFailure: CLError.Code

A constant that indicates the location manager can’t determine the heading.

static var rangingUnavailable: CLError.Code

A constant that indicates ranging is disabled.

static var rangingFailure: CLError.Code

A constant that indicates a general ranging error occurred.

