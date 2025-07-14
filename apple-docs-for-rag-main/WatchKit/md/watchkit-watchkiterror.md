

- WatchKit
-  WatchKitError 

Structure

# WatchKitError

An error reported by WatchKit.

watchOS

``` source
struct WatchKitError
```

## Topics

### Accessing Error Codes

static var downloadFailed: WatchKitError.Code

A download error.

static var invalidArgument: WatchKitError.Code

An invalid argument error.

static var mediaPlayerFailed: WatchKitError.Code

A media player error.

static var recordingFailed: WatchKitError.Code

An audio recording error.

static var unknown: WatchKitError.Code

An unknown error.

static var applicationDelegateWatchKitRequestReplyNotCalled: WatchKitError.Code

An unresponsive delegate error.

### Accessing the Error Domain

let WatchKitErrorDomain: String

The domain for WatchKit errors.

### Accessing Error Properties

enum Code

Error codes reported by WatchKit.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

