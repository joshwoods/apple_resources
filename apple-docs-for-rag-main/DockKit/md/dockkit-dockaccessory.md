

- DockKit
-  DockAccessory 

Class

# DockAccessory

Obtain accessory information and control tracking behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final class DockAccessory
```

## Overview

`DockAccessory` provides information about the dock accessory including its model name and firmware version. It also controls the dock accessory when you disable system tracking. Use `DockAccesory` to perform animations, or explicitly control the position of the dock accessory in three-dimensional space by supplying coordinates in units of radians. The collection of the X, Y, and Z values corresponding to pitch, yaw, and roll is the *angular position* of the dock accessory.

If there are multiple subjects in a video frame, direct the dock accessory to focus on a particular area of the frame using setFramingMode(_:).

Important

DockKit throws a DockKitError.frameRateTooHigh exception if you animate or set the orientation of the dock accessory too quickly, so keep call rates at 2 times per second or less.

## Topics

### Selecting and tracking

func selectSubject(at: CGPoint) async throws

Selects a subject to track at the supplied coordinates.

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

func track([DockAccessory.Observation], cameraInformation: DockAccessory.CameraInformation) async throws

Automatically generate and send tracking vectors to the device.

struct Observation

An observation of the contents of a single video frame.

struct CameraInformation

A collection of tracking information about the camera currently in use.

enum CameraOrientation

The set of camera orientations used to extract coordinates.

### Performing animation

func animate(motion: DockAccessory.Animation) async throws -> Progress

Starts an animation sequence.

func setRegionOfInterest(CGRect) async throws

Sets the area in the video frame in which the dock accessory tracks a subject.

var regionOfInterest: CGRect

The area in the video frame in which the dock accessory tracks a subject.

enum Animation

Character animations that describe how to move the dock accessory.

### Setting position and limits

func setLimits(DockAccessory.Limits) throws

Sets limits for the axes of rotation.

func setOrientation(Vector3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setOrientation(Rotation3D, duration: Duration, relative: Bool) throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

Deprecated

func setAngularVelocity(Vector3D) async throws

Sets the angular velocity of each axis of orientation.

### Setting framing mode

func setFramingMode(DockAccessory.FramingMode) async throws

Customize the dock accessory’s tracking behavior.

var framingMode: DockAccessory.FramingMode

The current framing mode.

enum FramingMode

The mode to control framing of the subject when tracking.

### Getting position and limits

var motionStates: DockAccessory.MotionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

var limits: DockAccessory.Limits

Current limits for the axes of rotation and maximum angular velocity.

struct MotionState

An event that indicates the state of a dock accessory’s current position and speed.

struct MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

struct Limits

Soft limits on multiple axes of rotation.

### Getting accessory information

var firmwareVersion: String?

The firmware version of the dock accessory.

var hardwareModel: String?

The model of the dock accessory.

let identifier: DockAccessory.Identifier

The name and unique identifer of the dock accessory.

struct Identifier

Information that uniquely identifies the dock accessory.

enum Category

Types of supported dock accesories.

enum State

The state of a dock accessory.

struct StateChange

An event that indicates a change in the state of a dock accessory.

struct StateChanges

An asynchronous sequence of dock accessory state changes.

### Inspecting the object

func hash(into: inout Hasher)

Creates a unique identifier representing the object.

var debugDescription: String

The text description of the dock accessory state.

### Structures

struct AccessoryEvents

An asynchronous sequence of dock accessory events.

struct BatteryState

A struct that represents an accessory battery state.

struct BatteryStates

An asynchronous sequence of dock accessory battery states.

struct TrackedObject

The state of a tracked object in the active tracking session.

struct TrackedPerson

The state of a tracked person in the active tracking session.

struct TrackingState

A representation of the active tracking session state.

struct TrackingStates

An asynchronous sequence of tracking session states.

### Operators

static func == (DockAccessory, DockAccessory) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var accessoryEvents: DockAccessory.AccessoryEvents

Events from the accessory that signify button presses or common camera controls.

var batteryStates: DockAccessory.BatteryStates

Battery states from the accessory that indicate changes in battery charge or readiness

var hashValue: Int

The hash value.

var trackingStates: DockAccessory.TrackingStates

Provides an access to the asynchronous sequence of tracking session states

### Instance Methods

func selectSubjects([UUID]) async throws

Selects subjects to track with specific identifiers

func setOrientation(Rotation3D, duration: Duration, relative: Bool) async throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

func setOrientation(Vector3D, duration: Duration, relative: Bool) async throws -> Progress

Sets the position of each axis of orientation to radians for pitch, yaw, and roll.

func track([DockAccessory.Observation], cameraInformation: DockAccessory.CameraInformation, image: CVPixelBuffer) async throws

Automatically generate and send tracking vectors to the device.

func track([AVMetadataObject], cameraInformation: DockAccessory.CameraInformation, image: CVPixelBuffer) async throws

Automatically generate and send tracking vectors to the device.

### Enumerations

enum AccessoryEvent

An enumeration that represents an accessory event.

enum BatteryChargeState

The charging state of an accessory battery

enum TrackedSubjectType

The subjects that the dock can track.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Controlling the dock accessory

Controlling a DockKit accessory using your camera app

Follow subjects in real time using an iPhone that you mount on a DockKit accessory.

class DockAccessoryManager

Observe the state of dock accessories and enable or disable system tracking.

enum DockKitError

A list of errors that DockKit sends.

