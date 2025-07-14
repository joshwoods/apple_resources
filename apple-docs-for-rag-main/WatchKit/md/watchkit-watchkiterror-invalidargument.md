

- WatchKit
- WatchKitError
-  invalidArgument 

Type Property

# invalidArgument

An invalid argument error.

watchOS

``` source
static var invalidArgument: WatchKitError.Code { get }
```

## Discussion

WatchKit reports this error when you specify invalid settings for one of the system supplied interfaces.

## See Also

### Accessing Error Codes

static var downloadFailed: WatchKitError.Code

A download error.

static var mediaPlayerFailed: WatchKitError.Code

A media player error.

static var recordingFailed: WatchKitError.Code

An audio recording error.

static var unknown: WatchKitError.Code

An unknown error.

static var applicationDelegateWatchKitRequestReplyNotCalled: WatchKitError.Code

An unresponsive delegate error.

