

- Push to Talk
-  Creating a Push to Talk app 

Article

# Creating a Push to Talk app

Build a walkie-talkie style app with system user interface controls.

## Overview

The Push to Talk (PTT) framework makes it easy to communicate with a group of individuals almost instantly with the press of a button. The framework provides your app with system user interface controls, as well as management for channel events. Handle push notifications and events like when audio transmission begins or ends, and when a person joins or leaves a channel.

PTT provides the interface, and you provide the back-end communication service. Its flexibility makes it compatible with your existing end-to-end communication solutions and backend infrastructure. Use PTT to integrate with Bluetooth accessories that trigger audio recording and transmission.

### Configure your Xcode project

To begin using the PTT framework, configure Xcode with the following steps:

1.  Choose your top-level project in the Xcode Project navigator.

2.  For your project’s target, choose Signing & Capabilities.

3.  Choose Editor \> Add Capability, select Background Modes, and select Push to Talk from the list of modes.

4.  Choose Editor \> Add Capability and select Push to Talk.

5.  Choose Editor \> Add Capability and select Push Notifications.

6.  Click Info, expand the Custom iOS Target Properties section, hover your pointer over a row and click the Add button (+). Enter the key name NSMicrophoneUsageDescription and a string value that explains why the app is requesting access to the device’s microphone.

### Join a channel

A channel represents and describes the PTT session to the system. Apps interact with channels through a PTChannelManager, which is the primary interface for joining channels and performing actions like transmitting and receiving audio. Multiple calls to channelManager(delegate:restorationDelegate:completionHandler:) result in the system returning the same shared instance, so store the channel manager in an instance variable.

```
```

Initialize the channel manager as soon as possible during startup to ensure the framework can restore existing channels and deliver push notifications to the app.

A PTChannelDescriptor describes the channel to the system so it can present details — like channel name and image — in the system UI.

```
```

The framework uses shared system resources, so only one PTT channel can be active on the system at a time. To join a channel, call requestJoinChannel(channelUUID:descriptor:). The system uses the same unique identifier when interacting with the manager throughout the life of the channel, so when joining a channel, store the descriptor and UUID for later use.

```
```

Important

A person can only join a channel when a PTT app is running in the foreground — with explicit user interaction — so apps need to provide buttons to allow a person to join and leave a channel.

After initializing the channel manager, the framework provides an ephemeral APNs device token in channelManager(_:receivedEphemeralPushToken:). Get the variable-length push token and send it to the app’s server. The token isn’t active until a person joins the channel. If they leave the channel, wait until they rejoin to resume notifications.

Joining a channel can fail when another channel is already active. On failure, the framework calls the delegate method channelManager(_:failedToJoinChannel:error:) and contains a PTChannelError.Code.

### Restore an active channel

When the system terminates an app or a person reboots the device, the app needs to restore active channels. Provide a channel descriptor to update the system in the PTChannelRestorationDelegate. The system only calls the restoration delegate method when it’s unable to use data it caches to restore a channel.

```
```

To keep the system responsive, return from channelDescriptor(restoredChannelUUID:) as soon as possible. Don’t perform long-running or blocking tasks — like network requests — to retrieve a descriptor.

### Set the channel transmission mode

After joining a channel, set the channel’s transmission mode to indicate when the user can transmit audio. The default transmission mode is PTTransmissionMode.halfDuplex, indicating that only one participant can send or receive audio at a time. The system prevents a person from transmitting audio while they’re receiving audio from a remote participant.

Use PTTransmissionMode.fullDuplex to allow a person to transmit and receive audio simultaneously. In full-duplex mode, the system allows a person to begin transmitting even if they’re receiving audio.

```
```

Set the transmission mode to PTTransmissionMode.listenOnly to prevent a participant from transmitting any audio.

### Report service status

If there are any platform service disruptions, report the service status through the channel manager. For example, if there’s a network outage, report that the connection is PTServiceStatus.connecting.

```
```

When the network is in a restored state, set the service status to PTServiceStatus.ready.

### Transmit audio

The framework provides flexibility in how apps handle audio transmission, and enables compatibility with other platforms. Apps implement their own audio encoding and streaming process to transmit audio between users. Start PTT transmissions from the system UI or by calling requestBeginTransmitting(channelUUID:). Begin transmission when the app is running in the foreground or following a characteristic change from a Core Bluetooth device.

The system automatically interprets play or pause toggle events from wired headsets and CarPlay devices when the system has an active PTT channel. Events result in begin- or end-transmission events in the PTT framework.

To begin a transmission, call requestBeginTransmitting(channelUUID:) with a unique channel identifier.

```
```

When the request to begin transmitting succeeds, the framework calls channelManager(_:channelUUID:didBeginTransmittingFrom:). The framework also calls this method if transmission begins from the system UI.

```
```

Before recording and transmitting audio, wait for the framework to call channelManager(_:didActivate:). The framework calls the method when the audio session is active. This allows for recording audio even if the app is in the background. The framework doesn’t call the method if the channel transmission mode is PTTransmissionMode.fullDuplex and already has an active audio session, because the app is receiving audio from a remote participant when a transmission begins.

```
```

Important

Let the system activate and deactivate the audio session to ensure it has the proper priority within the system.

The system provides built-in sound effects to indicate that the microphone is in an activated or deactivated state. Don’t provide sound effects for these events. The framework doesn’t support custom sound effects.

If the system can’t begin transmission — for example, if a person has an active cellular call — the framework calls channelManager(_:failedToBeginTransmittingInChannel:error:).

When transmission ends, the framework calls channelManager(_:channelUUID:didEndTransmittingFrom:) and channelManager(_:didDeactivate:). The system then returns the app to a suspended state if it’s running in the background. Use beginBackgroundTask(expirationHandler:) to request additional runtime to update the app’s server.

### Receive audio

The framework introduces a new APNs type for PTT apps. When an app’s server has new audio for a person to receive, it sends a PTT notification using the device push token that an app receives when joining a channel. A token is only active for the life of a channel, so an app receives a new token each time it joins a new channel.

Set the APNs push type to `pushtotalk` in the request header, and the topic header to the app’s bundle identifier with the `.voip-ptt` suffix. The payload can contain custom keys, such as the name of an active speaker or an indication that the session ended. Set the APNs priority to `10` to request immediate delivery, and set an expiration of `0` to prevent the system from delivering older pushes.

```
```

When the app’s server sends a PTT notification, the system starts the app in the background and calls incomingPushResult(channelManager:channelUUID:pushPayload:). When an app receives a push payload, it constructs a push result type to indicate what action to perform.

```
```

Return a PTPushResult as soon as possible and don’t block the thread. Perform network tasks — like downloading a speaker’s image or setting up a streaming network connection to a server — on a separate thread.

After setting activeRemoteParticipant(_:), the system activates the app’s audio session and calls the channelManager(_:didActivate:) method. When the app’s audio session is in an active state, begin playing back the audio it receives from the app’s server.

If the PTT channel transmission mode is PTTransmissionMode.halfDuplex, and the local participant is transmitting when the app receives a PTT notification, returning an active participant results in an error. End the local participant’s transmission by calling stopTransmitting(channelUUID:) before returning an active remote participant. The system batches these operations together — without deactivating the audio session — so an app can immediately begin playing audio it receives from a remote participant.

When an app is in the foreground, it can receive and queue messages for playback while playing messages it previously received.

When a remote participant finishes speaking, set setActiveRemoteParticipant(_:channelUUID:completionHandler:) to `nil` to indicate that the app is no longer receiving audio on the channel and the system can deactivate the audio session. This action updates the system UI and allows the user to transmit again.

### Reduce network latency and handle audio interruptions

To reduce the steps necessary to establish a secure TLS connection, and improve the initial connection speed, use the Network framework and implement `QUIC`. For more information about `QUIC`, see QUIC Options.

The system prioritizes communications from cellular, FaceTime, and VoIP calls, so PTT apps need to respond accordingly and handle failures gracefully. Monitor and respond to AVAudioSession notifications, such as session interruptions, route changes, and failures. For more information about handling interruptions, see Handling audio interruptions.

### Handle multiple Push to Talk conversations

To support simultaneous conversations, join a single channel and update the channel descriptor to reflect the active conversation. Call setChannelDescriptor(_:channelUUID:completionHandler:) to update the system UI when the active conversation changes.

When an app is in the process of receiving audio, use setActiveRemoteParticipant(_:channelUUID:completionHandler:) to update the system UI with new participant details when the conversation’s speaker changes. This eliminates having to send a new APNs notification.

## See Also

### Essentials

class PTChannelManager

An object that represents a push-to-talk channel manager.

