

- Game Controller
-  Letting players use their second-generation Siri Remote as a game controller 

Article

# Letting players use their second-generation Siri Remote as a game controller

Support the second-generation Siri Remote as a game controller in your Apple TV game.

## Overview

To add support for the second-generation Siri Remote in your Apple TV game, you make a few changes to your Xcode project and code.

### Configure your project

First configure your Xcode project to handle directional gamepads and multiple micro gamepads.

On the Signing & Capabilities tab in the project editor, add the Game Controllers capability to your project and check Directional Gamepad under Game Controllers. For more information, see Configuring game controllers.

On the Info tab, add the GCSupportsMultipleMicroGamepads key and set the value to `YES`. For more information, see Managing Your App’s Information Property List.

### Handle multiple micro gamepads

In your code, handle multiple micro gamepad connections. When a game controller connects, check if the controller is a directional gamepad using the isKind(of:) method:

```
if controller.microGamepad isKind(of: GCDirectionalGamepad.class) {
   ...
}
```

Check if the device category is second-generation Siri Remote using the productCategory property:

```
if device.productCategory == GCProductCategorySiriRemote2ndGen {
   ...
}
```

If these conditions are true, you can use the connected second-generation Siri Remote as a game controller.

### Access the remote buttons and directional pad

To access the center button of the second-generation Siri Remote, use the buttons property:

```
controller.physicalInputProfile.buttons[GCInputDirectionalCenterButton]
```

Then to access the directional pad, use the dpads property:

```
controller.physicalInputProfile.dpads[GCInputDirectionalCardinalDpad]
```

If your game requires an analog touch surface, check whether the directional pad is digital using the isAnalog property:

```
if physicalInputProfile.dpads[GCInputDirectionalDpad].isAnalog == false
```

For example, the Universal Electronic remote that works with Apple TV is a directional gamepad but with physical non-analog buttons.

## See Also

### Game controllers

Supporting Game Controllers

Support a physical controller or add a virtual controller to enhance how people interact with your game through haptics, lighting, and motion sensing.

protocol GCDevice

A protocol that defines a common interface for game input devices.

class GCController

A representation of a real game controller, a virtual controller, or a snapshot of a controller.

class GCRacingWheel

An object that represents a physical racing wheel controller connected to a device.

class GCKeyboard

An object that represents a physical keyboard connected to a device.

class GCMouse

An object that represents a physical mouse connected to a device.

