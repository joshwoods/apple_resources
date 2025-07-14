

- RoomPlan
-  RoomCaptureSessionDelegate 

Protocol

# RoomCaptureSessionDelegate

A specification of important events in the room-scanning process.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
protocol RoomCaptureSessionDelegate : AnyObject
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

The room-capture session’s delegate property is of this type.

## Topics

### Beginning a session

func captureSession(RoomCaptureSession, didStartWith: RoomCaptureSession.Configuration)

Notifies the delegate when the session starts.

**Required** Default implementation provided.

### Updating a session

func captureSession(RoomCaptureSession, didAdd: CapturedRoom)

Notifies the delegate of newly added surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

session has recently removed surfaces and objects

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

Notifies the delegate when the session changes the dimensions and the transform properties of surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Notifies the delegate when the session updates the scan results.

**Required** Default implementation provided.

### Coaching the user

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

Notifies the delegate of an instruction to display to the user.

**Required** Default implementation provided.

### Completing a session

func captureSession(RoomCaptureSession, didEndWith: CapturedRoomData, error: (any Error)?)

Notifies the delegate of completion with either scan results or an error.

**Required** Default implementation provided.

### Default implementations

func captureSession(RoomCaptureSession, didStartWith: RoomCaptureSession.Configuration)

Provides a default, blank implementation for when the session starts.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Provides a default, blank implementation for when the session updates surfaces and objects during a scan.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

Provides a default, blank implementation for when the session removes surfaces and objects.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

session has changed dimensions and transform properties of surfaces and objects

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

session has user guidance instructions

func captureSession(RoomCaptureSession, didEndWith: CapturedRoomData, error: (any Error)?)

session ends with either CapturedRoom or error

## See Also

### Scanning Protocol

class RoomCaptureSession

An object that manages the room-scanning process.

