

- Foundation
- URLSessionDownloadTask
-  init() Deprecated

Initializer

# init()

Initializes a download task.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
init()
```

Deprecated

Please use -\[NSURLSession downloadTaskWithRequest:\] or other NSURLSession methods to create instances

## Discussion

Don’t use this initalizer to manually create download tasks. Instead, use the factory methods on URLSession to add tasks to an existing URL session.

## See Also

### Creating download tasks

class func new() -> Self

Creates and initializes a download task.

Deprecated

