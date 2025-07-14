

- Nearby Interaction
-  NISessionDelegate 

Protocol

# NISessionDelegate

An object that monitors and reacts to session updates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
protocol NISessionDelegate : NSObjectProtocol
```

## Mentioned in 

Initiating and maintaining a session

## Overview

Assign a delegate that Nearby Interaction can use to notify your app of important events that occur during the session life cycle.

## Topics

### Reacting to session start

func sessionDidStartRunning(NISession)

Notifies the app when a session starts or resumes running.

### Monitoring peers

func session(NISession, didUpdate: [NINearbyObject])

Notifies you when the session updates nearby objects.

func session(NISession, didGenerateShareableConfigurationData: Data, for: NINearbyObject)

Provides configuration data to share with a third-party accessory.

func session(NISession, didRemove: [NINearbyObject], reason: NINearbyObject.RemovalReason)

Notifies you when the session removes one or more nearby objects.

enum RemovalReason

The reason a session removed a nearby object.

### Managing interruption

func sessionWasSuspended(NISession)

Notifies you of a suspended session.

func sessionSuspensionEnded(NISession)

Notifies you of the end of a session’s suspension.

### Handling errors

func session(NISession, didInvalidateWith: any Error)

Notifies you of an invalidated session.

### Coaching the user

func session(NISession, didUpdateAlgorithmConvergence: NIAlgorithmConvergence, for: NINearbyObject?)

Provides recommended actions the user can take to facilitate the framework’s Camera Assistance.

enum NIAlgorithmConvergenceStatus

The possible states of Camera Assistance.

struct Reason

The possible reasons for the Camera Assistance status.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Periodic updates

class NINearbyObject

Location information for a peer device in an interaction session.

