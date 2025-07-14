

- ScreenCaptureKit
-  SCStreamError 

Structure

# SCStreamError

An instance representing a ScreenCaptureKit framework error.

Mac Catalyst 18.2+macOS 12.3+

``` source
struct SCStreamError
```

## Overview

Important

When a user cancels a stream, the system calls an observer’s stream(_:didStopWithError:) method with SCStreamError.Code.userStopped. Rather than treating this event as an error, handle it as an intentional user request.

## Topics

### Error inspection

Error Constants

Error code constants for framework operations.

enum Code

Codes for user cancellation events and errors that can occur in ScreenCaptureKit.

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Stream errors

let SCStreamErrorDomain: String

A string representation of the error domain.

