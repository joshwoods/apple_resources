

- Core Location
- CLLocationPushServiceError
-  CLLocationPushServiceError.Code 

Enumeration

# CLLocationPushServiceError.Code

Error codes the location manager returns if starting to monitor for location push notifications fails.

iOS 15.0+iPadOS 15.0+

``` source
enum Code
```

## Overview

These error codes are returned from startMonitoringLocationPushes(completion:)

## Topics

### Getting the error code

case unknown

An error code that indicates the app was unable to start the location push service for an unknown reason.

case missingPushExtension

An error code that indicates the app is missing a Location Push Service Extension.

case missingPushServerEnvironment

An error code that indicates the app is missing an Apple Push Notification service (APNs) environment entitlement.

case missingEntitlement

An error code that indicates the app is missing the entitlement it needs to use the location push service.

case unsupportedPlatform

An error code that indicates the location push service isn’t available on this platform.

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

### Location push service extension

com.apple.developer.location.push

An entitlement to enable a location-sharing app to query someone’s location in response to a push notification.

protocol CLLocationPushServiceExtension

The interface you adopt in the type that acts as the main entry point for a Location Push Service Extension.

struct CLLocationPushServiceError

Error codes the location manager returns if starting to monitor for location push notifications fails.

let CLLocationPushServiceErrorDomain: String

The domain for Location Push Service Extension errors.

