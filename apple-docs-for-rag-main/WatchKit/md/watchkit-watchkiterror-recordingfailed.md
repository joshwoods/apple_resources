

- WatchKit
- WatchKitError
-  recordingFailed 

Type Property

# recordingFailed

An audio recording error.

watchOS

``` source
static var recordingFailed: WatchKitError.Code { get }
```

## Discussion

WatchKit reports this error when it’s unable to record audio using the audio recording interface.

## See Also

### Accessing Error Codes

static var downloadFailed: WatchKitError.Code

A download error.

static var invalidArgument: WatchKitError.Code

An invalid argument error.

static var mediaPlayerFailed: WatchKitError.Code

A media player error.

static var unknown: WatchKitError.Code

An unknown error.

static var applicationDelegateWatchKitRequestReplyNotCalled: WatchKitError.Code

An unresponsive delegate error.

