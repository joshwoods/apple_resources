

- os
- AnimationFormatString
-  AnimationFormatString.OSLogMessage 

Structure

# AnimationFormatString.OSLogMessage

A log message that includes an animation tag.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogMessage
```

## Overview

An AnimationFormatString.OSLogMessage structure contains a message that you construct from a string interpolation or string literal. This message includes an additional animation tag. Don’t create this structure directly. The system creates one automatically when you log a message using the os_signpost(_:dso:log:name:signpostID:_:_:) function

## Topics

### Creating a Format String

init(stringLiteral: String)

Creates a log message using a string literal.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

