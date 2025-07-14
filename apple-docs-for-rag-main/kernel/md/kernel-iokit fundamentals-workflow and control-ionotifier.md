

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IONotifier 

Class

# IONotifier

An abstract base class defining common methods for controlling a notification request.

macOS 10.0+

``` source
class IONotifier : OSObject
```

## Overview

IOService notification requests are represented as implementations of the IONotifier object. It defines methods to enable, disable and remove notification requests. These actions are synchronized with invocations of the notification handler, so removing a notification request will guarantee the handler is not being executed.

## Topics

### Miscellaneous

disable

Disables the notification request.

enable

Sets the enable state of the notification request.

remove

Removes the notification request and releases it.

### Instance Methods

- disable

- enable

- getMetaClass

- remove

## Relationships

### Inherits From

- OSObject

## See Also

### Notifications

IOServiceNotificationDispatchSource

IOServiceNotificationDispatchSourceInterface

