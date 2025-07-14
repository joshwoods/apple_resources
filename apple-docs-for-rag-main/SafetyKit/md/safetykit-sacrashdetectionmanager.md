

- SafetyKit
-  SACrashDetectionManager 

Class

# SACrashDetectionManager

Provides registration and management of Crash Detection events.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
class SACrashDetectionManager
```

## Overview

Use this class to determine Crash Detection availabilty on iPhone, detect authorization status, and register for Crash Detection events. Not all iPhones support Crash Detection, so verify that isAvailable returns true.

Check the value of authorizationStatus to determine if the person designates this app on their iPhone to receive Crash Detection events. If the value is not SAAuthorizationStatus.authorized, set delegate and call requestAuthorization(completionHandler:) to request authorization.

After your app has authorization to receive Crash Detection events, adopt SACrashDetectionDelegate and implement crashDetectionManager(_:didDetect:). If a vehicular crash occurs, the system calls the method with the Crash Detection event.

## Topics

### Determining availability

class var isAvailable: Bool

A Boolean value that indicates if Crash Detection is available.

var authorizationStatus: SAAuthorizationStatus

A value that indicates if the person authorized the app to receive Crash Detection events.

### Requesting authorization

var delegate: (any SACrashDetectionDelegate)?

The object that receives Crash Detection events.

func requestAuthorization(completionHandler: (SAAuthorizationStatus, (any Error)?) -> Void)

Requests permission to access Crash Detection information.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Detecting a crash

enum SAAuthorizationStatus

An enumeration that represents the current Crash Detection event authorization state.

class SACrashDetectionEvent

Describes the information about a vehicular crash.

protocol SACrashDetectionDelegate

The protocol that an object adopts to receive Crash Detection events and changes to the authorization status.

