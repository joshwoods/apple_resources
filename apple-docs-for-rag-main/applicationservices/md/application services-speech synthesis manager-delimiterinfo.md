

- Application Services
- Speech Synthesis Manager
-  DelimiterInfo 

Structure

# DelimiterInfo

Defines a delimiter information structure.

macOS 10.0+

``` source
struct DelimiterInfo
```

## Overview

A delimiter information structure defines the characters used to indicate the beginning and end of a command embedded in text. A delimiter can be one or two characters.

Ordinarily, applications that support embedded speech commands should not change the start or end delimiters. However, if for some reason you must change the delimiters, you can use the `SetSpeechInfo` function with the `soCommandDelimiter` selector. For example, you might do this if a text buffer naturally includes the delimiter strings. Before passing such a buffer to the Speech Synthesis Manager, you can change the delimiter strings to some two-character sequences not used in the buffer and then change the delimiter strings back once processing of the buffer is complete.

If a single-byte delimiter is desired, it should be followed by a `NULL` (0) byte. If the delimiter strings both consist of two `NULL` bytes, embedded command processing is disabled.

## Topics

### Initializers

init()

init(startDelimiter: (UInt8, UInt8), endDelimiter: (UInt8, UInt8))

### Instance Properties

var endDelimiter: (UInt8, UInt8)

The end delimiter for an embedded command. By default, the end delimiter is “`]]`”.

var startDelimiter: (UInt8, UInt8)

The start delimiter for an embedded command. By default, the start delimiter is “`[[`”.

