

- ClockKit
-  CLKWatchFaceLibrary 

Class

# CLKWatchFaceLibrary

An object for importing watch faces that the app provides.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.0+

``` source
class CLKWatchFaceLibrary
```

## Mentioned in 

Sharing an Apple Watch face

## Overview

Use a CLKWatchFaceLibrary object to add an existing .`watchface` file to the Watch app. Add watch faces only on devices that support pairing with an Apple Watch.

## Topics

### Importing a Watch Face

func addWatchFace(at: URL, completionHandler: ((any Error)?) -> Void)

Adds a watch face from the app’s bundle.

### Handling Errors

class let ErrorDomain: String

The domain for errors while importing watch faces.

enum ErrorCode

Error codes that the watch face library returns.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Face Sharing

Sharing an Apple Watch face

Distribute a customized watch face to Apple Watch users.

