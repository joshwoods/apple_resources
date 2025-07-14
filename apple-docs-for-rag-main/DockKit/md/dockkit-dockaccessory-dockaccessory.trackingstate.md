

- DockKit
- DockAccessory
-  DockAccessory.TrackingState 

Structure

# DockAccessory.TrackingState

A representation of the active tracking session state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct TrackingState
```

## Overview

The active tracking session emits this state 10 times per second.

## Topics

### Instance Properties

var description: String

var time: Date

The timestamp indicating when the dock captured the tracking state.

var trackedSubjects: [DockAccessory.TrackedSubjectType]

A collection of actively tracked subjects.

## Relationships

### Conforms To

- Sendable

