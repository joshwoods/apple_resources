

- WatchKit
- WatchKitError
-  mediaPlayerFailed 

Type Property

# mediaPlayerFailed

A media player error.

watchOS

``` source
static var mediaPlayerFailed: WatchKitError.Code { get }
```

## Discussion

WatchKit reports this error when it’s unable to play a media file.

## See Also

### Accessing Error Codes

static var downloadFailed: WatchKitError.Code

A download error.

static var invalidArgument: WatchKitError.Code

An invalid argument error.

static var recordingFailed: WatchKitError.Code

An audio recording error.

static var unknown: WatchKitError.Code

An unknown error.

static var applicationDelegateWatchKitRequestReplyNotCalled: WatchKitError.Code

An unresponsive delegate error.

