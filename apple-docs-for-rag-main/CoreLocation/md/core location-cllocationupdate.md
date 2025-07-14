

- Core Location
-  CLLocationUpdate 

Structure

# CLLocationUpdate

A structure that contains the location information the framework delivers with each update.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CLLocationUpdate
```

## Mentioned in 

Handling location updates in the background

## Overview

You use `CLLocationUpate` events to observe changes in the device’s location, and to determine the activity type.

## Topics

### Determining movement and location

var isStationary: Bool

A Boolean value that indicates whether the user is stationary.

Deprecated

var location: CLLocation?

The user’s location, if available.

### Receiving location updates

static func liveUpdates(CLLocationUpdate.LiveConfiguration) -> CLLocationUpdate.Updates

Tells Core Location to start delivering the location updates it produces for the configuration you specify.

enum LiveConfiguration

Values for indicating the kind of updates the framework delivers.

struct Updates

A structure that represents an asynchronous sequence of location updates.

### Instance Properties

var accuracyLimited: Bool

var authorizationDenied: Bool

var authorizationDeniedGlobally: Bool

var authorizationRequestInProgress: Bool

var authorizationRestricted: Bool

var insufficientlyInUse: Bool

var locationUnavailable: Bool

var serviceSessionRequired: Bool

var stationary: Bool

## Relationships

### Conforms To

- Sendable

## See Also

### Essentials

Configuring your app to use location services

Prepare your app to start collecting location data.

Supporting live updates in SwiftUI and Mac Catalyst apps

Enable background events by adding lifecycle event support.

class CLLocationManager

The object you use to start and stop the delivery of location-related events to your app.

class CLBackgroundActivitySession

An object that manages a visual indicator that keeps your app in use in the background, allowing it to receive updates or events.

Adopting live updates in Core Location

Simplify location delivery using asynchronous events in Swift.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

