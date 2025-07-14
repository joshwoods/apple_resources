

- Core Location
- CLLocationUpdate
-  CLLocationUpdate.Updates 

Structure

# CLLocationUpdate.Updates

A structure that represents an asynchronous sequence of location updates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Updates
```

## Overview

CLLocationUpdate uses this structure to asynchronously deliver a stream of location updates to your app when you call liveUpdates(_:).

## Topics

### Type aliases

struct Iterator

The type of the update’s iterator.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Receiving location updates

static func liveUpdates(CLLocationUpdate.LiveConfiguration) -> CLLocationUpdate.Updates

Tells Core Location to start delivering the location updates it produces for the configuration you specify.

enum LiveConfiguration

Values for indicating the kind of updates the framework delivers.

