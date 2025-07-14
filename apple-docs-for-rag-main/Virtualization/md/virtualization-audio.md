

- Virtualization
-  Audio 

API Collection

# Audio

Configure audio devices that enable the guest operating system to perform audio playback and capture through the host’s audio devices.

## Overview

If your app can configure an audio input device, you must set an NSMicrophoneUsageDescription message in your app’s `Info.plist.` The system uses this description when asking the user’s permission to enable microphone access. If this message isn’t set or the key isn’t present, the system denies microphone access to your app.

Note

To enable VIRTIO sound support in Linux guests, configure sound support in the kernel using the `CONFIG_SND_VIRTIO` kernel parameter.

You can add audio support to your guest with just a few lines of code. The example below shows how to configure a VM to expose a VIRTIO sound device that consists of an audio input and output on the guest that the system bridges to the host machine’s speakers and microphone:

- Swift
- Objective-C

```
let outputStream = VZVirtioSoundDeviceOutputStreamConfiguration()
outputStream.sink = VZHostAudioOutputStreamSink()
let outputSoundDevice = VZVirtioSoundDeviceConfiguration()
outputSoundDevice.streams = [outputStream]

let inputStream = VZVirtioSoundDeviceInputStreamConfiguration()
inputStream.source = VZHostAudioInputStreamSource()
let inputSoundDevice = VZVirtioSoundDeviceConfiguration()
inputSoundDevice.streams = [inputStream]

let configuration = VZVirtualMachineConfiguration()
configuration.audioDevices = [outputSoundDevice, inputSoundDevice]
```

```
VZVirtioSoundDeviceOutputStreamConfiguration *outputStream = [[VZVirtioSoundDeviceOutputStreamConfiguration alloc] init];
outputStream.sink = [[VZHostAudioOutputStreamSink alloc] init];
VZVirtioSoundDeviceConfiguration *outputSoundDevice = [[VZVirtioSoundDeviceConfiguration alloc] init];
soundDevice.streams = @[ outputStream ];

VZVirtioSoundDeviceInputStreamConfiguration *inputStream = [[VZVirtioSoundDeviceInputStreamConfiguration alloc] init];
inputStream.source = [[VZHostAudioInputStreamSource alloc] init];
VZVirtioSoundDeviceConfiguration *inputSoundDevice = [[VZVirtioSoundDeviceConfiguration alloc] init];
soundDevice.streams = @[ inputStream ];

VZVirtualMachineConfiguration *configuration = [[VZVirtualMachineConfiguration alloc] init];
configuration.audioDevices = @[ outputSoundDevice, inputSoundDevice ];
```

## Topics

### Configurations

class VZVirtioSoundDeviceConfiguration

An object that defines a Virtio sound device configuration.

class VZVirtioSoundDeviceOutputStreamConfiguration

An object that defines a Virtio sound device output stream configuration.

class VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

class VZAudioDeviceConfiguration

The base class for an audio device configuration.

class VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

### Audio streams

class VZHostAudioOutputStreamSink

Host audio output stream sink plays audio to the host system’s default output device.

class VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

class VZAudioInputStreamSource

The base class for an audio input stream source.

## See Also

### Devices

Graphics

Configure a device for a guest to display its UI.

Keyboards and pointing devices

Configure devices that connect a mouse and keyboard to the guest system.

Memory

Configure a memory balloon device to change the allocated memory for the guest system.

Network

Configure the devices that connect the guest system to the network.

Randomization

Configure a device for the guest system to use to generate random numbers.

Serial ports

Configure the serial devices that you use to communicate with the guest system.

Shared directories

Configure devices that share directories from the host into the guest system.

Sockets

Configure a device that manages port-based communication with the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

