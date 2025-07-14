

- AVFAudio
- AVAudioSession
- AVAudioSession.Port
-  bluetoothLE 

Type Property

# bluetoothLE

An output to a Bluetooth Low Energy (LE) device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let bluetoothLE: AVAudioSession.Port
```

## Discussion

Apple supports the use of Bluetooth Low Energy (LE) hearing aids. Apps don’t have control over routing to these devices. Instead, the system automatically decides when routing to Bluetooth LE is appropriate.

To determine if audio is being routed to a Bluetooth LE device, inspect the current audio route and look for the presence of a Bluetooth LE port, as shown in the following code example.

```
var routingToBLE = false
let session = AVAudioSession.sharedInstance()
// Iterate over the currentRoute's outputs.
for portDesc in session.currentRoute.outputs where portDesc.portType == .bluetoothLE {
    routingToBLE = true
    break
}
```

## See Also

### Getting Output Ports

static let airPlay: AVAudioSession.Port

An output to an AirPlay device.

static let bluetoothA2DP: AVAudioSession.Port

An output to a Bluetooth A2DP device.

static let builtInReceiver: AVAudioSession.Port

An output to the speaker you hold to your ear when you’re on a phone call.

static let builtInSpeaker: AVAudioSession.Port

An output to the device’s built-in speaker.

static let HDMI: AVAudioSession.Port

An output to a High-Definition Multimedia Interface (HDMI) device.

static let headphones: AVAudioSession.Port

An output to wired headphones.

static let lineOut: AVAudioSession.Port

A line-level output to the dock connector.

