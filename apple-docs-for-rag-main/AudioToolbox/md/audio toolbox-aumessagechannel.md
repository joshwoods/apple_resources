

- Audio Toolbox
-  AUMessageChannel 

Protocol

# AUMessageChannel

A specification for a bidirectional communication message channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
protocol AUMessageChannel
```

## Overview

Audio units and their hosts have unique communication needs. For example, for better audio processing they can exchange musical context. An audio unit implements a class that conforms to AUMessageChannel and returns an instance from messageChannel(for:). A host queries the instance through the channel name.

This protocol offers a method to send messages to an audio unit and a block to send messages to the host.

## Topics

### Sending a Message to an Audio Unit

func callAudioUnit([AnyHashable : Any]) -> [AnyHashable : Any]

Sends an audio unit a custom data message.

### Sending a Message to a Host

var callHostBlock: CallHostBlock?

A callback for the audio unit to send a message to the host.

## See Also

### Messaging Channels

func messageChannel(for: String) -> any AUMessageChannel

Returns an object for bidirectional communication between an audio unit and its host.

