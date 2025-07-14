

- SafetyKit
- SACrashDetectionEvent
-  SACrashDetectionEvent.Response 

Enumeration

# SACrashDetectionEvent.Response

An enumeration that defines possible emergency responses to a Crash Detection event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
enum Response
```

## Overview

The Crash Detection event response indicates whether the system attempted to dial the Emergency SOS - Call After Severe Crash provider, depending on the setting in the Settings app.

## Topics

### Determining responses

case attempted

The system attempted to dial the Emergency SOS - Call After Severe Crash provider.

case disabled

The system couldn’t contact the Emergency SOS - Call After Severe Crash provider because the feature is off in the Settings app.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responding to a crash

class SAEmergencyResponseManager

Provides actions in response to a Crash Detection event.

protocol SAEmergencyResponseDelegate

The interface for receiving updates about a requested emergency response action.

