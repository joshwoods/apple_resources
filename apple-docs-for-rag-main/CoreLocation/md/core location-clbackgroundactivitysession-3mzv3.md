

- Core Location
-  CLBackgroundActivitySession 

Class

# CLBackgroundActivitySession

An object that manages a visual indicator that keeps your app in use in the background, allowing it to receive updates or events.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+watchOS 10.0+

``` source
final class CLBackgroundActivitySession
```

## Mentioned in 

Handling location updates in the background

Supporting live updates in SwiftUI and Mac Catalyst apps

## Overview

Use `CLBackgroundActivitySession` to start a background activity session that allows a when-in-use authorized app to receive location updates or monitoring events.

## Topics

### Creating a background activity session

init()

Creates a new background activity session.

### Ending the session

func invalidate()

Invalidates the background activity session.

### Classes

class Diagnostics

### Structures

struct Diagnostic

### Instance Properties

var diagnostics: CLBackgroundActivitySession.Diagnostics

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

struct CLLocationUpdate

A structure that contains the location information the framework delivers with each update.

Adopting live updates in Core Location

Simplify location delivery using asynchronous events in Swift.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

