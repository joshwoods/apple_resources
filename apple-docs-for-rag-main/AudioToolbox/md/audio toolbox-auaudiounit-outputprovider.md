

- Audio Toolbox
- AUAudioUnit
-  outputProvider 

Instance Property

# outputProvider

The block that the output unit will call to get audio to send to the output.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var outputProvider: AURenderPullInputBlock? { get set }
```

## Discussion

This block must be set if output is enabled.

## See Also

### Configuring the Device

var deviceID: AUAudioObjectID

Gets the I/O hardware device.

func setDeviceID(AUAudioObjectID) throws

Sets the I/O hardware device.

var canPerformInput: Bool

Determines whether the I/O device can perform input.

var canPerformOutput: Bool

Determines whether the I/O device can perform output.

var isInputEnabled: Bool

A flag enabling audio input from the unit.

var isOutputEnabled: Bool

A flag enabling audio output from the unit.

var inputHandler: AUInputHandler?

The block that the output unit will call to notify when input is available.

var deviceInputLatency: TimeInterval

The audio device’s input latency, in seconds.

var deviceOutputLatency: TimeInterval

The audio devic’s output latency, in seconds.

func startHardware() throws

Starts the audio hardware.

func stopHardware()

Stops the audio hardware.

typealias AURenderPullInputBlock

A block to supply audio input to a render block.

