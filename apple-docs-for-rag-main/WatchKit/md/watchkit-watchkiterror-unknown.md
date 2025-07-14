

- WatchKit
- WatchKitError
-  unknown 

Type Property

# unknown

An unknown error.

watchOS

``` source
static var unknown: WatchKitError.Code { get }
```

## Discussion

WatchKit reports this error when it can’t determine the precise reason for the failure.

## See Also

### Accessing Error Codes

static var downloadFailed: WatchKitError.Code

A download error.

static var invalidArgument: WatchKitError.Code

An invalid argument error.

static var mediaPlayerFailed: WatchKitError.Code

A media player error.

static var recordingFailed: WatchKitError.Code

An audio recording error.

static var applicationDelegateWatchKitRequestReplyNotCalled: WatchKitError.Code

An unresponsive delegate error.

