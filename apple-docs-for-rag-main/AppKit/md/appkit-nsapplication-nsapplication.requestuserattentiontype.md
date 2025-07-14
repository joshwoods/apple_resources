

- AppKit
- NSApplication
-  NSApplication.RequestUserAttentionType 

Enumeration

# NSApplication.RequestUserAttentionType

These constants specify the level of severity of a user attention request and are used by cancelUserAttentionRequest(_:) and requestUserAttention(_:).

macOS

``` source
enum RequestUserAttentionType
```

## Topics

### Constants

case criticalRequest

The user attention request is a critical request.

case informationalRequest

The user attention request is an informational request.

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

func cancelUserAttentionRequest(Int)

Cancels a previous user attention request.

func reply(toOpenOrPrint: NSApplication.DelegateReply)

Handles errors that might occur when the user attempts to open or print files.

enum DelegateReply

Constants that indicate whether a copy or print operation was successful, was canceled, or failed.

