

- Core MIDI
-  MIDICIProfileResponderDelegate Deprecated

Protocol

# MIDICIProfileResponderDelegate

A protocol that defines the methods to respond to MIDI-CI responder life-cycle events.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
protocol MIDICIProfileResponderDelegate : NSObjectProtocol
```

Deprecated

No longer supported for CoreMIDI

## Topics

### Protocol Methods

func connectInitiator(MIDICIInitiatiorMUID, with: MIDICIDeviceInfo) -> Bool

Enables a MIDI-CI initiator to create a session or reject the connection attempt.

**Required**

func handleData(for: MIDICIProfile, onChannel: MIDIChannelNumber, data: Data)

Processes MIDI data for a profile and channel.

func willSetProfile(MIDICIProfile, onChannel: MIDIChannelNumber, enabled: Bool) -> Bool

Provides an opportunity to perform an action before the system sets the profile.

func initiatorDisconnected(MIDICIInitiatiorMUID)

Provides an opportunity to perform an action after the system disconnects the initiator.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting a Responder Delegate

var profileDelegate: any MIDICIProfileResponderDelegate

The profile delegate.

Deprecated

