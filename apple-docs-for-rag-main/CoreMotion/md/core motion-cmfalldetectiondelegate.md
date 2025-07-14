

- Core Motion
-  CMFallDetectionDelegate 

Protocol

# CMFallDetectionDelegate

A delegate that receives information about fall detection events and authorization status changes.

watchOS 7.2+

``` source
protocol CMFallDetectionDelegate : NSObjectProtocol
```

## Topics

### Detecting Falls

func fallDetectionManager(CMFallDetectionManager, didDetect: CMFallDetectionEvent, completionHandler: () -> Void)

Indicates a fall detection event occurred.

### Detecting Authorization Changes

func fallDetectionManagerDidChangeAuthorization(CMFallDetectionManager)

Indicates the fall detection authorization status changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Fall detection

class CMFallDetectionManager

An object for managing fall detection events.

class CMFallDetectionEvent

An object that contains data about a fall detection event.

NSFallDetectionUsageDescription

A message to the user that explains the app’s request for permission to access fall detection event data.

