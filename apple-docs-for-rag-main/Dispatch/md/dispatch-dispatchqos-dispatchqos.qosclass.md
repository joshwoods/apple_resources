

- Dispatch
- DispatchQoS
-  DispatchQoS.QoSClass 

Enumeration

# DispatchQoS.QoSClass

Quality-of-service classes that specify the priorities for executing tasks.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum QoSClass
```

## Overview

Use quality-of-service classes to communicate the intent behind the work that your app performs. The system uses those intentions to determine the best way to execute your tasks given the available resources. For example, the system gives higher priority to threads that contain user-interactive tasks to ensure that those tasks are executed quickly. Conversely, it gives lower priority to background tasks, and may attempt to save power by executing them on more power-efficient CPU cores. The system determines how to execute your tasks dynamically based on system conditions and the tasks you schedule.

## Topics

### Getting the Quality-of-Service Class

case userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updating your app’s user interface.

case userInitiated

The quality-of-service class for tasks that prevent the user from actively using your app.

case `default`

The default quality-of-service class.

case utility

The quality-of-service class for tasks that the user does not track actively.

case background

The quality-of-service class for maintenance or cleanup tasks that you create.

case unspecified

The absence of a quality-of-service class.

### Initializing the Type

init?(rawValue: qos_class_t)

Initializes the type with a raw value.

var rawValue: qos_class_t

The value of the raw type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a QoS Structure

init(qosClass: DispatchQoS.QoSClass, relativePriority: Int)

Creates a new `DispatchQoS` object with the specified QoS class and relative priority.

