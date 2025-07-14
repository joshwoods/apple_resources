

- Kernel
- Hardware Families
-  HID 

API Collection

# HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

## Overview

The use of kernel extensions for HID drivers is deprecated. Instead, create a DriverKit extension using HIDDriverKit.

## Topics

### Reports

IOHIDReportType

Describes different type of HID reports.

HIDReportCommandType

IOHIDCompletion

Struct specifying action to perform when set/get report completes.

IOHIDCompletionAction

Function called when set/get report completes

### Event Types

IOHIDBiometricEventType

IOHIDPointerEventOptions

IOHIDOptionsType

Options for opening a device via IOHIDLib.

IOHIDStandardType

Type to define what industrial standard the device is referencing.

IOHIDValueScaleType

Describes different types of scaling that can be performed on element values.

IOHIDKeyboardEventOptions

IOHIDScrollEventOptions

IOHIDEventType

### HID Elements

IOHIDElementCollectionType

Describes different types of HID collections.

IOHIDElementCommitDirection

IOHIDElementCookie

Abstract data type used as a unique identifier for an element.

IOHIDElementFlags

IOHIDElementType

Describes different types of HID elements.

IOHIDValueOptions

Describes options for gathering element values.

### HID Types

IOHIDButtonModes

IOHIDDigitizerStylusData

IOHIDDigitizerTouchData

IOHIDQueueOptionsType

Options for creating a queue via IOHIDLib.

NXByteOrder

NXEQElement

NXEvent

NXEventData

NXEventExt

NXEventExtension

NXEventPtr

NXEventSystemDevice

NXEventSystemDeviceList

NXEventSystemInfoData

NXEventSystemInfoType

NXKeyMapping

NXMouseButton

NXMouseScaling

NXParsedKeyMapping

NXSwappedDouble

NXSwappedFloat

NXTabletPointData

NXTabletPointDataPtr

NXTabletProximityData

NXTabletProximityDataPtr

## See Also

### Interfaces

Audio

Implement a driver that interacts with audio hardware.

Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

