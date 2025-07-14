

- Audio Toolbox
- AUAudioUnit
-  isInputEnabled 

Instance Property

# isInputEnabled

A flag enabling audio input from the unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var isInputEnabled: Bool { get set }
```

## Discussion

The default value is false.

If your audio unit desires input audio, this property must be set to true and the value of canPerformInput must also be true.

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

var isOutputEnabled: Bool

A flag enabling audio output from the unit.

var inputHandler: AUInputHandler?

The block that the output unit will call to notify when input is available.

var outputProvider: AURenderPullInputBlock?

The block that the output unit will call to get audio to send to the output.

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

