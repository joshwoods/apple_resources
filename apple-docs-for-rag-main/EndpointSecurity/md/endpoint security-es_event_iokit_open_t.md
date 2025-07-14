

- Endpoint Security
-  es_event_iokit_open_t 

Structure

# es_event_iokit_open_t

A type for an event that indicates the opening of an IOKit device.

Mac CatalystmacOS

``` source
struct es_event_iokit_open_t
```

## Overview

Endpoint Security generates this event when a process calls IOServiceOpen(_:_:_:_:) in order to open a communications channel with an IOKit driver. The event doesn’t correspond to driver/device communication and provides neither visibility nor access control into devices.

## Topics

### Inspecting Event Properties

var user_client_class: es_string_token_t

The name of the IOKit service client.

var user_client_type: UInt32

The type of the IOKit client.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init()

init(user_client_type: UInt32, user_client_class: es_string_token_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Kernel Event Types

struct es_event_kextload_t

A type for an event that indicates the loading of a kernel extension.

struct es_event_kextunload_t

A type for an event that indicates the unloading of a Kernel Extension (KEXT).

