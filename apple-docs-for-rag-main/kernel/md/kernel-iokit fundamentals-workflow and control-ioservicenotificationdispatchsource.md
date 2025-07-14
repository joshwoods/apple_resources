

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOServiceNotificationDispatchSource 

Class

# IOServiceNotificationDispatchSource

DriverKitKernelDriverKit 19.0+macOS 10.15.4+

**DriverKit**

``` source
class IOServiceNotificationDispatchSource : IODispatchSource
```

**macOS**

``` source
class IOServiceNotificationDispatchSource : IODispatchSource, IOServiceNotificationDispatchSourceInterface
```

## Topics

### Instance Methods

- Cancel

- Cancel_Impl

- CheckForWork

- CheckForWork_Impl

- CopyNextNotification

- CopyNextNotification

- CopyNextNotification_Impl

- DeliverNotifications

- Dispatch

- ServiceNotificationReady

- ServiceNotificationReady

- SetEnableWithCompletion

- SetEnableWithCompletion_Impl

- SetHandler

- SetHandler

- SetHandler_Impl

- free

- getMetaClass

- init

### Type Methods

+ CopyNextNotification_Invoke

+ Create

+ Create_Call

+ Create_Impl

+ Create_Invoke

+ ServiceNotificationReady_Invoke

+ ServiceNotificationReady_Invoke

+ SetHandler_Invoke

## Relationships

### Inherits From

- IODispatchSource
- IODispatchSource
- IOServiceNotificationDispatchSourceInterface

## See Also

### Notifications

IOServiceNotificationDispatchSourceInterface

IONotifier

An abstract base class defining common methods for controlling a notification request.

