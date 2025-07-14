

- Core Location
-  CLError 

Structure

# CLError

A Core Location error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CLError
```

## Overview

Instances of NSError object delivered to the delegate use these error codes for the code property of the error object.

## Topics

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

enum Code

Error codes returned by the location manager object.

### Getting region monitoring errors

static var regionMonitoringDenied: CLError.Code

A constant that indicates the user denied access to the region monitoring service.

static var regionMonitoringFailure: CLError.Code

A constant that indicates the location manager failed to monitor a registered region.

static var regionMonitoringSetupDelayed: CLError.Code

A constant that indicates Core Location couldn’t initialize the region monitoring feature immediately.

static var regionMonitoringResponseDelayed: CLError.Code

A constant that indicates Core Location will deliver events but they may be delayed.

### Getting geocoding errors

static var geocodeCanceled: CLError.Code

A constant that indicates the geocode request was canceled.

static var geocodeFoundNoResult: CLError.Code

A constant that indicates the geocode request yielded no result.

static var geocodeFoundPartialResult: CLError.Code

A constant that indicates the geocode request yielded a partial result.

### Getting deferred location update errors

static var deferredFailed: CLError.Code

A constant that indicates the location manager didn’t enter deferred mode for an unknown reason.

static var deferredCanceled: CLError.Code

A constant that indicates your app or the location manager canceled the request for deferred updates.

static var deferredAccuracyTooLow: CLError.Code

A constant that indicates deferred mode isn’t supported for the requested accuracy.

static var deferredDistanceFiltered: CLError.Code

A constant that indicates deferred mode doesn’t support distance filters.

static var deferredNotUpdatingLocation: CLError.Code

A constant that indicates the location manager didn’t enter deferred mode because location updates were already disabled or paused.

### Getting the error details

var alternateRegion: CLRegion?

A region that location services can monitor more effectively.

### Type Properties

static var historicalLocationError: CLError.Code

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let kCLErrorDomain: String

The domain for Core Location errors.

let kCLErrorUserInfoAlternateRegionKey: String

A key in the user information dictionary of an error relating to a delayed region-monitoring response.

