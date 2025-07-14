

- Core HID
- HIDUsage
-  HIDUsage.LEDUsage 

Enumeration

# HIDUsage.LEDUsage

macOS 15.0+

``` source
enum LEDUsage
```

## Topics

### Enumeration Cases

case batteryLow

case batteryOK

case batteryOperation

case blueLEDChannel

case busy

case callPickup

case cameraOff

case cameraOn

case capsLock

case cav

case clv

case compose

case conference

case coverage

case dataMode

case doNotDisturb

case equalizerEnable

case error

case externalPowerConnected

case fastBlinkOffTime

case fastBlinkOnTime

case fastForward

case flashOnTime

case forward

case genericIndicator

case goodStatus

case greenLEDChannel

case headset

case highCutFilter

case hold

case indicatorAmber

case indicatorBlue

case indicatorFastBlink

case indicatorFlash

case indicatorGreen

case indicatorOff

case indicatorOn

case indicatorOrange

case indicatorRed

case indicatorSlowBlink

case kana

case ledIntensity

case lowCutFilter

case messageWaiting

case microphone

case mute

case nightMode

case numLock

case offHook

case offLine

case onLine

case paperJam

case paperOut

case pause

case play

case player1

case player2

case player3

case player4

case player5

case player6

case player7

case player8

case playerIndicator

case power

case ready

case record

case recordingFormatDetect

case redLEDChannel

case remote

case repeatTrack

case reverse

case rewind

case rgbLED

case ring

case samplingRateDetect

case scrollLock

case sendCalls

case shift

case slowBlinkOffTime

case slowBlinkOnTime

case soundFieldOn

case speaker

case spinning

case standBy

case stereo

case stop

case surroundOn

case systemMicrophoneMute

case systemSuspend

case toneEnable

case usageInUseIndicator

case usageIndicatorColor

case usageMultiModeIndicator

case usageSelectedIndicator

case warningStatus

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

