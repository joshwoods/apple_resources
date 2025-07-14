

- Matter
-  MTRDeviceControllerDelegate 

Protocol

# MTRDeviceControllerDelegate

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
protocol MTRDeviceControllerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func controller(MTRDeviceController, commissioningComplete: (any Error)?)Deprecated

func controller(MTRDeviceController, commissioningComplete: (any Error)?, nodeID: NSNumber?)

func controller(MTRDeviceController, commissioningComplete: (any Error)?, nodeID: NSNumber?, metrics: MTRMetrics)

func controller(MTRDeviceController, commissioningSessionEstablishmentDone: (any Error)?)

func controller(MTRDeviceController, readCommissioningInfo: MTRProductIdentity)Deprecated

func controller(MTRDeviceController, statusUpdate: MTRCommissioningStatus)

func controller(MTRDeviceController, read: MTRCommissioneeInfo)

Notify the delegate when commissioning infomation has been read from the commissionee.

func controller(MTRDeviceController, suspendedChangedTo: Bool)

Notify the delegate when the suspended state changed of the controller, after this happens the controller will be in the specified state.

func devicesChanged(for: MTRDeviceController)

Notify the delegate when the list of MTRDevice objects in memory has changed.

## Relationships

### Inherits From

- NSObjectProtocol

