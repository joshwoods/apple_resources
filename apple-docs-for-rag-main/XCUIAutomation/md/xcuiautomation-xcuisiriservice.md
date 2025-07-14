

- XCUIAutomation
-  XCUISiriService 

Class

# XCUISiriService

A proxy that simulates a device’s Siri interface.

iOS 10.3+iPadOS 10.3+Mac Catalyst 10.3+Xcode 16.3+

``` source
@MainActor
class XCUISiriService
```

## Overview

This class allows issuing textual queries and producing element queries for UI shown by Siri.

## Topics

### Siri activation

func activate(voiceRecognitionText: String)

Presents the Siri UI, if it’s not currently active, and accepts a string that is then processed as if it’s recognized speech.

### Siri proxy state

var debugDescription: String

Provides debugging information about the element representing the root of the Siri UI.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- XCUIElementTypeQueryProvider

## See Also

### Related Documentation

var siriService: XCUISiriService

An object that represents the Siri interface on the device.

### Device simulation

class XCUIDevice

A proxy that can simulate physical buttons, device orientation, and Siri interaction for an iOS, watchOS, or tvOS device.

class XCUISystem

A proxy that provides an interface to OS-specific properties and actions.

