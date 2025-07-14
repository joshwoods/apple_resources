

- AVFAudio
-  AVAudioSessionRouteDescription 

Class

# AVAudioSessionRouteDescription

An object that describes the input and output ports associated with a session’s audio route.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioSessionRouteDescription
```

## Mentioned in 

Responding to audio route changes

## Overview

You don’t create instances of this class yourself. Instead, you retrieve the current audio route from your app’s AVAudioSession object.

## Topics

### Getting the Input and Output Ports

var inputs: [AVAudioSessionPortDescription]

An array of audio input port descriptions.

var outputs: [AVAudioSessionPortDescription]

An array of audio output port descriptions.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Inspecting the current route

var currentRoute: AVAudioSessionRouteDescription

A description of the current audio route’s input and output ports.

class AVAudioSessionPortDescription

Information about the capabilities of the port and the hardware channels it supports.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

