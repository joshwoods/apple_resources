

- AppKit
- NSApplication
-  NSApplication.DelegateReply 

Enumeration

# NSApplication.DelegateReply

Constants that indicate whether a copy or print operation was successful, was canceled, or failed.

macOS

``` source
enum DelegateReply
```

## Overview

These constants are used by the reply(toOpenOrPrint:) method.

## Topics

### Constants

case success

Indicates the operation succeeded.

case cancel

Indicates the user cancelled the operation.

case failure

Indicates an error occurred processing the operation.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing User Attention Requests

func requestUserAttention(NSApplication.RequestUserAttentionType) -> Int

Starts a user attention request.

enum RequestUserAttentionType

These constants specify the level of severity of a user attention request and are used by cancelUserAttentionRequest(_:) and requestUserAttention(_:).

func cancelUserAttentionRequest(Int)

Cancels a previous user attention request.

func reply(toOpenOrPrint: NSApplication.DelegateReply)

Handles errors that might occur when the user attempts to open or print files.

