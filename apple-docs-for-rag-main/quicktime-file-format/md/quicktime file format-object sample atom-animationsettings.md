

- QuickTime File Format
- Object sample atom
-  animationSettings 

Data field

# animationSettings

A set of 32-bit flags that encode information about the animation settings of the object.

## Overview

The `animationSettings` field of the object sample atom is a long integer that specifies a set of animation settings for an object node. Animation settings specify characteristics of the movie while it is playing. Use these constants to specify animation settings:

```
enum QTVRAnimationSettings {
    kQTVRObjectAnimateViewFramesOn              = (1 

**Constant Descriptions**

`kQTVRObjectAnimateViewFramesOn`  
The animation setting to play all frames in the current view state.

`kQTVRObjectPalindromeViewFramesOn`  
The animation setting to play a back-and-forth animation of the frames of the current view state.

`kQTVRObjectStartFirstViewFrameOn`  
The animation setting to play the frame animation starting with the first frame in the view (that is, at the view start time).

`kQTVRObjectAnimateViewsOn`  
The animation setting to play all views of the current object in the default row of views.

`kQTVRObjectPalindromeViewsOn`  
The animation setting to play a back-and-forth animation of all views of the current object in the default row of views.

`kQTVRObjectSyncViewToFrameRate`  
The animation setting to synchronize the view animation to the frame animation and use the same options as for frame animation.

`kQTVRObjectDontLoopViewFramesOn`  
The animation setting to stop playing the frame animation in the current view at the end.

`kQTVRObjectPlayEveryViewFrameOn`  
The animation setting to play every view frame regardless of play rate. The play rate is used to adjust the duration in which a frame appears but no frames are skipped so the rate is not exact.

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

