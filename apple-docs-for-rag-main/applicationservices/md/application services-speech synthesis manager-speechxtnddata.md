

- Application Services
- Speech Synthesis Manager
-  SpeechXtndData 

Structure

# SpeechXtndData

Defines a speech extension data structure.

macOS 10.0+

``` source
struct SpeechXtndData
```

## Overview

The speech extension data structure allows you to use the GetSpeechInfo and SetSpeechInfo functions with selectors defined by particular synthesizers. By requiring that you pass to one of these functions a pointer to a speech extension data structure, synthesizers can permit the exchange of data in any format.

## Topics

### Initializers

init()

init(synthCreator: OSType, synthData: (UInt8, UInt8))

### Instance Properties

var synthCreator: OSType

The synthesizer’s creator ID, identical to the value stored in the `synthManufacturer` field of a speech version information structure. You should set this field to the appropriate value before calling `GetSpeechInfo` or `SetSpeechInfo`.

var synthData: (UInt8, UInt8)

Synthesizer-specific data. The size and format of the data in this field may vary.

