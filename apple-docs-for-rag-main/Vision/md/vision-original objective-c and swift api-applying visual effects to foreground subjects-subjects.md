

- Vision
- Original Objective-C and Swift API
-  Applying visual effects to foreground subjects 

Sample Code

# Applying visual effects to foreground subjects

Segment the foreground subjects of an image and composite them to a new background with visual effects.

Download

iOS 17.0+iPadOS 17.0+Xcode 15.0+

## Overview

Note

This sample code project is associated with WWDC23 session 10176: Lift subjects from images in your app.

### Configure the sample code project

Before you run the sample code project in Xcode, set the run destination to an iOS 17 device.

## See Also

### Image background removal

class VNInstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

class VNGenerateForegroundInstanceMaskRequest

A request that generates an instance mask of noticable objects to separate from the background.

let VNGenerateForegroundInstanceMaskRequestRevision1: Int

A constant for specifying the first revision of the foreground instance mask request.

