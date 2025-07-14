

- Audio Toolbox
- AUAudioUnit
-  startHardware() 

Instance Method

# startHardware()

Starts the audio hardware.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func startHardware() throws
```

## Discussion

- false if the operation failed.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

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

var outputProvider: AURenderPullInputBlock?

The block that the output unit will call to get audio to send to the output.

var deviceInputLatency: TimeInterval

The audio device’s input latency, in seconds.

var deviceOutputLatency: TimeInterval

The audio devic’s output latency, in seconds.

func stopHardware()

Stops the audio hardware.

typealias AURenderPullInputBlock

A block to supply audio input to a render block.

