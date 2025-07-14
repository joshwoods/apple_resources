

- Core Services
- Apple Events
-  Priority Constants for the AESend Function (Deprecated in macOS) 

# Priority Constants for the AESend Function (Deprecated in macOS)

Specify a value for the `sendPriority` parameter of the `AESend` function.

## Overview

For related information, see the `AESend(_:_:_:_:_:_:_:)` function and AESendMode.

### Version-Notes

The `sendPriority` parameter of the `AESend` function is deprecated in macOS.

## Topics

### Constants

var kAENormalPriority: Int

The Apple Event Manager posts the event at the end of the event queue of the server process and the server processes the Apple event as soon as it has the opportunity.

var kAEHighPriority: Int

The Apple Event Manager posts the event at the beginning of the event queue of the server process.

