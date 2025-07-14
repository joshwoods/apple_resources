

- ReplayKit
-  RPBroadcastActivityViewControllerDelegate 

Protocol

# RPBroadcastActivityViewControllerDelegate

The protocol you implement to respond to changes to a broadcast activity user interface.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
protocol RPBroadcastActivityViewControllerDelegate : NSObjectProtocol
```

## Overview

Use this class to respond to changes to a broadcast activity user interface, represented by an RPBroadcastActivityViewController object.

## Topics

### Connecting to a Service

func broadcastActivityViewController(RPBroadcastActivityViewController, didFinishWith: RPBroadcastController?, error: (any Error)?)

Indicates that the broadcast activity view controller is ready to be dismissed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the Delegate

var delegate: (any RPBroadcastActivityViewControllerDelegate)?

The delegate for the broadcast activity view controller.

