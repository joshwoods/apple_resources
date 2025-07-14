

- Core Services
- Carbon Core
- Unicode Utilities
-  UCKeyLayoutFeatureInfo 

Structure

# UCKeyLayoutFeatureInfo

Specifies the longest possible output string to be produced by the current `'uchr'` resource.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct UCKeyLayoutFeatureInfo
```

## Overview

The Unicode keyboard-layout ( `'uchr'`) resource contains the data necessary to map virtual key codes to Unicode character codes for a given keyboard layout. The `'uchr'` format consists of a header information section and five key mapping data sections. The `UCKeyLayoutFeatureInfo` type is used in the header section of the `'uchr'` resource.

## Topics

### Initializers

init()

init(keyLayoutFeatureInfoFormat: UInt16, reserved: UInt16, maxOutputStringLength: UInt32)

### Instance Properties

var keyLayoutFeatureInfoFormat: UInt16

An unsigned 16-bit integer identifying the format of the `UCKeyLayoutFeatureInfo` structure. Set to `kUCKeyLayoutFeatureInfoFormat`.

var maxOutputStringLength: UInt32

An unsigned 32-bit integer specifying the longest possible output string of Unicode characters to be produced by this `'uchr'` resource.

var reserved: UInt16

Reserved. Set to 0.

