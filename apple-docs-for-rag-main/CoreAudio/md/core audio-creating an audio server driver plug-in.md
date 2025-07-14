

- Core Audio
-  Creating an Audio Server Driver Plug-in 

Sample Code

# Creating an Audio Server Driver Plug-in

Build a virtual audio device by creating a custom driver plug-in.

Download

macOS 12.0+Xcode 13.0+

## Overview

This sample shows how to create a minimal Audio Server plug-in. Written in standard C, the sample provides the minimal implementation you need to publish a single, functioning audio device to the system. The audio device provides the following features:

- Configurable device primary volume, muting, and data sources

- 44.1 kHz and 48 kHz sample rates

- Two channels of audio I/O in 32-bit, floating point, linear PCM format

Install the sample’s `.driver` bundle to `/Library/Audio/Plug-Ins/HAL` and reboot your computer. Use Audio MIDI Setup to inspect the newly installed device.

## See Also

### Drivers

Building an Audio Server Plug-in and Driver Extension

Create a plug-in and driver extension to support an audio device in macOS.

Capturing system audio with Core Audio taps

Use a Core Audio tap to capture outgoing audio from a process or group of processes.

