

- QuickTime File Format
- Object sample atom
-  controlSettings 

Data field

# controlSettings

A set of 32-bit flags that encode information about the control settings of the object.

## Overview

The `controlSettings` field of the object sample atom is a long integer that specifies a set of control settings for an object node. Control settings specify whether the object can wrap during panning and tilting, as well as other features of the node. The control settings are specified using these bit flags:

```
enum QTVRControlSettings {
    kQTVRObjectWrapPanOn                        = (1 

**Constant Descriptions**

`kQTVRObjectWrapPanOn`  
The control setting to enable wrapping during panning. When this control setting is enabled, the user can wrap around from the current pan constraint maximum value to the pan constraint minimum value (or vice versa) using the mouse or arrow keys.

`kQTVRObjectWrapTiltOn`  
The control setting to enable wrapping during tilting. When this control setting is enabled, the user can wrap around from the current tilt constraint maximum value to the tilt constraint minimum value (or vice versa) using the mouse or arrow keys.

`kQTVRObjectCanZoomOn`  
The control setting to enable zooming. When this control setting is enabled, the user can change the current field of view using the zoom-in and zoom-out keys on the keyboard (or using the VR controller buttons).

`kQTVRObjectReverseHControlOn`  
The control setting to reverse the direction of the horizontal control.

`kQTVRObjectReverseVControlOn`  
The control setting to reverse the direction of the vertical control.

`kQTVRObjectSwapHVControlOn`  
The control setting to exchange the horizontal and vertical controls.

`kQTVRObjectTranslationOn`  
The control setting to enable translation. When this setting is enabled, the user can translate using the mouse when either the translate key is held down or the controller translation mode button is toggled on.

## See Also

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

movieType

The movie controller type.

viewStateCount

The number of view states of the object.

defaultViewState

The 1-based index of the default view state.

mouseDownViewState

The 1-based index of the mouse-down view state.

viewDuration

The total movie duration of all image frames contained in an object’s view.

columns

The number of columns in the object image array.

rows

The number of rows in the object image array.

mouseMotionScale

The mouse motion scale factor.

minPan

The minimum pan angle, in degrees.

maxPan

The maximum pan angle, in degrees.

defaultPan

The default pan angle, in degrees.

minTilt

The minimum tilt angle, in degrees.

maxTilt

The maximum tilt angle, in degrees.

