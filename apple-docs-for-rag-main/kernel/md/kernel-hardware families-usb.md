

- Kernel
- Hardware Families
-  USB 

API Collection

# USB

Implement a driver that supports Universal Serial Bus (USB) devices.

## Overview

Use kernel extensions to implement support for devices with real-time requirements, such as audio and video devices.

Important

For most types of USB drivers, Apple has deprecated the use of kernel extensions. Instead, create a DriverKit extension using USBDriverKit.

This framework refers to the USB Implementers Forum (USB-IF) *Universal Serial Bus 3.2 Specification*, Revision 1.0, September 22, 2017. You can view this specification and other referenced USB specifications at http://www.usb.org/.

## Topics

### Device Communication

Building a Simple USB Driver

Set up and load a driver that logs output to the Console app.

IOUSBHostIOSourceClientRecordLink

A structure that represents a USB host input/output source client record entry.

IOUSBHostIOSourceClientRecordList

A structure that represents a list of USB host input/output source client records.

### USB Specifications

IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

USB Device Descriptors

Structures and functions for working with device descriptors.

Additional Specifications

Structures related to hubs, devices, and endpoints.

### Actions

IOUSBCompletionAction

A function the system calls when the USB input/output request completes.

IOUSBCompletion

The structure that specifies the action to perform when the USB input/output request completes.

IOUSBHostBundledCompletion

The structure that specifies the action to perform when a bulk USB input/output request completes.

IOUSBHostBundledCompletionAction

The function description for a USB host bundled completion action.

IOUSBHostCompletion

The structure that specifies the action to perform when the USB input/output request completes.

IOUSBHostCompletionAction

The function description for a USB host completion action.

IOUSBHostIsochronousCompletion

A structure describing the completion callback for an asynchronous isochronous operation.

IOUSBHostIsochronousCompletionAction

The function description for a USB host isochronous completion action.

IOUSBIsocCompletion

A structure specifying the action to perform when an isochronous USB input/output operation completes.

IOUSBIsocCompletionAction

The function that executes when the isochronous USB input/output request completes.

IOUSBLowLatencyIsocCompletion

The function that executes when the low-latency isochronous USB input/output request completes.

IOUSBLowLatencyIsocCompletionAction

The function that excutes when the low-latency isochronous USB input/output request completes.

IOUSBCompletionActionWithTimeStamp

The function that executes when the USB input/output request completes.

IOUSBCompletionWithTimeStamp

A structure specifying action to perform when the USB input/output request completes.

## See Also

### Hardware Interconnects

ATA

Implement a driver that supports Advanced Technology Attachment (ATA) devices.

Bluetooth

Implement a driver that supports Bluetooth devices.

FireWire

Implement a driver that supports FireWire devices.

PCI

Implement a driver that supports Thunderbolt devices or PCI cards.

