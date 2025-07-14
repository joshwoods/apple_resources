

- ARKit
-  ARSessionObserver 

Protocol

# ARSessionObserver

Methods you can implement to respond to changes in the state of an AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol ARSessionObserver : NSObjectProtocol
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Overview

This protocol defines optional methods common to the ARSessionDelegate, ARSCNViewDelegate, and ARSKViewDelegate protocols. You can implement this protocol’s methods when adopting one of those protocols.

## Topics

### Responding to Tracking Quality Changes

func session(ARSession, cameraDidChangeTrackingState: ARCamera)

Informs the delegate of changes to the quality of ARKit’s device position tracking.

func session(ARSession, didChange: ARGeoTrackingStatus)

Listen and react to geo-tracking state changes.

### Handling Interruptions

func sessionWasInterrupted(ARSession)

Tells the delegate that the session has temporarily stopped processing frames and tracking device position.

func sessionInterruptionEnded(ARSession)

Tells the delegate that the session has resumed processing frames and tracking device position.

func sessionShouldAttemptRelocalization(ARSession) -> Bool

Asks the delegate whether to attempt recovery of world-tracking state after an interruption.

### Receiving Audio Data

func session(ARSession, didOutputAudioSampleBuffer: CMSampleBuffer)

Tells the delegate that a new sample buffer of recorded audio is available.

### Handling Errors

func session(ARSession, didFailWithError: any Error)

Tells the delegate that the session has stopped running due to an error.

let ARErrorDomain: String

The domain for error objects produced by an AR session.

### Managing Collaboration

func session(ARSession, didOutputCollaborationData: ARSession.CollaborationData)

Provides information for nearby users about your perspective in the environment.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- ARSCNViewDelegate
- ARSKViewDelegate
- ARSessionDelegate

## See Also

### Responding to events

var delegate: (any ARSessionDelegate)?

An object you provide to receive captured video images and tracking information, or to respond to changes in session status.

var delegateQueue: dispatch_queue_t?

The dispatch queue through which the session calls your delegate methods.

protocol ARSessionDelegate

Methods you can implement to receive captured video frame images and tracking state from an AR session.

