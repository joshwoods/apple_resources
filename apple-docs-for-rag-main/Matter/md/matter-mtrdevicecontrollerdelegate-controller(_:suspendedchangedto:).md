

- Matter
- MTRDeviceControllerDelegate
-  controller(\_:suspendedChangedTo:) 

Instance Method

# controller(\_:suspendedChangedTo:)

Notify the delegate when the suspended state changed of the controller, after this happens the controller will be in the specified state.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
optional func controller(
    _ controller: MTRDeviceController,
    suspendedChangedTo suspended: Bool
)
```

