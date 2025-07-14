

- CarPlay
-  CPPointOfInterestTemplateDelegate 

Protocol

# CPPointOfInterestTemplateDelegate

The methods to handle a Point of Interest template’s events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol CPPointOfInterestTemplateDelegate : NSObjectProtocol
```

## Overview

You use the `CPPointOfInterestTemplateDelegate` protocol to respond to a Point of Interest template’s events. The protocol defines methods that CarPlay calls in response to these events, and your implementation provides the appropriate behavior for when the events occur. For example, when the user pans the template’s map and the visible region changes, update the points of interest that the template displays to only those relevant to the new region.

## Topics

### Responding to Map Region Changes

func pointOfInterestTemplate(CPPointOfInterestTemplate, didChangeMapRegion: MKCoordinateRegion)

Tells the delegate about changes to the visible region of the template’s map.

**Required**

### Responding to Point of Interest Selection

func pointOfInterestTemplate(CPPointOfInterestTemplate, didSelectPointOfInterest: CPPointOfInterest)

Tells the delegate when the user selects a point of interest.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling Template Events

var pointOfInterestDelegate: (any CPPointOfInterestTemplateDelegate)?

The object that serves as the template’s delegate.

