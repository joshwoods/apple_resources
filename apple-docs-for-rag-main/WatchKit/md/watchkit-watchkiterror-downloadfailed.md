

- WatchKit
- WatchKitError
-  downloadFailed 

Type Property

# downloadFailed

A download error.

watchOS

``` source
static var downloadFailed: WatchKitError.Code { get }
```

## Discussion

WatchKit reports this error when it can’t download a media file.

## See Also

### Accessing Error Codes

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

