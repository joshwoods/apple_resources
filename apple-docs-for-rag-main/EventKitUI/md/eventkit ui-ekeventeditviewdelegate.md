

- EventKit UI
-  EKEventEditViewDelegate 

Protocol

# EKEventEditViewDelegate

A notification sent to the delegate when the user finishes editing an event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol EKEventEditViewDelegate : NSObjectProtocol
```

## Overview

Delegates of an EKEventEditViewController object conform to this protocol. Use `EKEventEditViewController` to allow the user to either create an event or edit an existing event. To be notified when the user finishes editing the event, set the delegate to an object conforming to this protocol.

## Topics

### Getting the Default Calendar

func eventEditViewControllerDefaultCalendar(forNewEvents: EKEventEditViewController) -> EKCalendar

The default calendar to use when creating new events.

### Finishing an Edit

func eventEditViewController(EKEventEditViewController, didCompleteWith: EKEventEditViewAction)

Invoked when the user finishes editing an event.

**Required**

enum EKEventEditViewAction

The action taken by the user after editing an event.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the Event Editing Interface

var editViewDelegate: (any EKEventEditViewDelegate)?

The delegate to notify when editing an event.

