

- HealthKit
- HKAttachmentDataReader
-  progress 

Instance Property

# progress

An object you can use to track the progress while reading an attachment’s data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
var progress: Progress { get }
```

## See Also

### Reading attachment data

var data: Data

The abstract’s data.

var bytes: HKAttachment.AsyncBytes

An asynchronous sequence that provides the attachment’s data.

