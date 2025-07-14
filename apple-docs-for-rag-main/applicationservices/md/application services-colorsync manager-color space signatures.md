

- Application Services
- ColorSync Manager
-  Color Space Signatures 

# Color Space Signatures

Define four-character-sequences associated with color spaces.

## Overview

A ColorSync profile header contains a `dataColorSpace` field that carries the signature of the data color space in which the color values in an image using the profile are expressed. This enumeration defines the signatures for the color spaces supported by ColorSync for version 2.x profiles.

## Topics

### Constants

var cmXYZData: Int

The XYZ data color space.

var cmLabData: Int

The L\*a\*b\* data color space.

var cmLuvData: Int

The L\*u\*v\* data color space.

var cmYCbCrData: Int

var cmYxyData: Int

The Yxy data color space.

var cmRGBData: Int

The RGB data color space.

var cmSRGBData: Int

var cmGrayData: Int

The Gray data color space.

var cmHSVData: Int

The HSV data color space.

var cmHLSData: Int

The HLS data color space.

var cmCMYKData: Int

The CMYK data color space.

var cmCMYData: Int

The CMY data color space.

var cmMCH5Data: Int

The five-channel multichannel (HiFi) data color space.

var cmMCH6Data: Int

The six-channel multichannel (HiFi) data color space.

var cmMCH7Data: Int

The seven-channel multichannel (HiFi) data color space.

var cmMCH8Data: Int

The eight-channel multichannel (HiFi) data color space.

var cm3CLRData: Int

var cm4CLRData: Int

var cm5CLRData: Int

var cm6CLRData: Int

var cm7CLRData: Int

var cm8CLRData: Int

var cm9CLRData: Int

var cm10CLRData: Int

var cm11CLRData: Int

var cm12CLRData: Int

var cm13CLRData: Int

var cm14CLRData: Int

var cm15CLRData: Int

var cmNamedData: Int

