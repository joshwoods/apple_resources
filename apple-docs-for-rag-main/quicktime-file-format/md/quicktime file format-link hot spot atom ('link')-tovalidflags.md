

- QuickTime File Format
- Link hot spot atom ('link')
-  toValidFlags 

Data field

# toValidFlags

A set of flags that indicate which destination node view settings are valid.

## Overview

Specifies which view settings are to be used when moving to a destination node from a hot spot. You can use these bit flags to specify a value for that field:

```
enum {
    kQTVRValidPan                               = 1 

**Constant Descriptions**

`kQTVRValidPan`  
The setting for using the destination pan angle.

`kQTVRValidTilt`  
The setting for using the destination tilt angle.

`kQTVRValidFOV`  
The setting for using the destination field of view.

`kQTVRValidViewCenter`  
The setting for using the destination view center.

## See Also

### Data fields

majorVersion

The major version number of the file format.

minorVersion

The minor version number of the file format.

toNodeID

The ID of the destination node.

fromValidFlags

A set of flags that indicate which source node view settings are valid.

fromPan

The preferred from-pan angle at the source node.

fromTilt

The preferred from-tilt angle at the source node.

fromFOV

The preferred from-field of view at the source node.

fromViewCenter

The preferred from-view center at the source node.

toPan

The pan angle to use when displaying the destination node.

toTilt

The tilt angle to use when displaying the destination node.

toFOV

The field of view to use when displaying the destination node.

toViewCenter

The view center to use when displaying the destination node.

distance

The distance between the source node and the destination node.

flags

A set of link hot spot flags.

reserved1

Reserved.

