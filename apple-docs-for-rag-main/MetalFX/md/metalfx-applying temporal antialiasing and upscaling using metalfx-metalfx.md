

- MetalFX
-  Applying temporal antialiasing and upscaling using MetalFX 

Sample Code

# Applying temporal antialiasing and upscaling using MetalFX

Reduce render workloads while increasing image detail with MetalFX.

Download

iOS 16.0+iPadOS 16.0+macOS 13.0+Xcode 14.0+

## Overview

Note

This sample code project is associated with WWDC22 session 10103: Boost performance with MetalFX upscaling.

### Configure the sample code project

This sample code project requires the following:

- macOS 13 or later, and a Mac with the M1 chip or an Intel-based Mac

- iOS 16 or later, and an iPad with the M1 chip

- Xcode 14 or later

## See Also

### Temporal scaling

protocol MTLFXTemporalScaler

An upscaling effect that generates a higher resolution texture in a render pass by analyzing multiple input textures over time.

class MTLFXTemporalScalerDescriptor

A set of properties that configure a temporal scaling effect, and a factory method that creates the effect.

