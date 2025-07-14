

- EventKit UI
-  EKEventViewDelegate 

Protocol

# EKEventViewDelegate

Delegates used to display details for calendar events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol EKEventViewDelegate : NSObjectProtocol
```

## Overview

Delegates of an EKEventViewController object conform to this protocol. Notifies the event view controller’s delegate when closing the event view controller. It is your responsibility to close the event view controller and perform any additional tasks within this protocol’s method.

## Topics

### Responding to the Interface’s Dismissal

enum EKEventViewAction

Describes the action taken to close the event view controller.

func eventViewController(EKEventViewController, didCompleteWith: EKEventViewAction)

Invoked when closing the event view controller.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Dismissing the Event Interface

var delegate: (any EKEventViewDelegate)?

The event view controller’s delegate.

