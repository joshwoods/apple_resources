

- Core HID
- HIDUsage
-  HIDUsage.TelephonyDeviceUsage 

Enumeration

# HIDUsage.TelephonyDeviceUsage

macOS 15.0+

``` source
enum TelephonyDeviceUsage
```

## Topics

### Enumeration Cases

case activateHandsetAudio

case addressBookID

case alertSoundConfirm

case alertSoundError

case alertSoundNotification

case alternateFunction

case answerOnOrOff

case answeringMachine

case callDuration

case callWaitingTone

case callerID

case conference

case confirmationTone1

case confirmationTone2

case doNotDisturb

case drop

case dualModePhone

case emailMessageWaiting

case feature

case flash

case forwardCalls

case handset

case handsetNickname

case headset

case hold

case hookSwitch

case hostAvailable

case hostCallActive

case hostControl

case hostHold

case hostRingTone

case incomingCallHistory

case incomingCallHistoryCount

case insideDialTone

case insideRingTone

case insideRingback

case line

case lineBusyTone

case message

case messageControls

case outgoingCallHistory

case outgoingCallHistoryCount

case outsideDialTone

case outsideRingTone

case outsideRingback

case park

case phone

case phoneCallHistoryKey

case phoneCallerIDKey

case phoneDateDay

case phoneDateMonth

case phoneDateYear

case phoneDirectory

case phoneKey0

case phoneKey1

case phoneKey2

case phoneKey3

case phoneKey4

case phoneKey5

case phoneKey6

case phoneKey7

case phoneKey8

case phoneKey9

case phoneKeyA

case phoneKeyB

case phoneKeyC

case phoneKeyD

case phoneKeyPound

case phoneKeyStar

case phoneLocale

case phoneMute

case phoneSettingsKey

case phoneTimeHour

case phoneTimeMinute

case phoneTimeSecond

case priorityRingTone

case priorityRingback

case programmableButton

case pstnRingTone

case reDialablePhoneNumber

case recallNumber

case redial

case reorderTone

case ringEnable

case ringSelect

case ringType

case ringer

case screenCalls

case send

case silentRing

case speakerPhone

case speedDial

case stopRingTone

case storeNumber

case telephonyKeyPad

case tonesOff

case transfer

case voiceMail

case voicemailMessageWaiting

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

