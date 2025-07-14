

- StoreKit
- SKPaymentQueue
-  start(\_:) Deprecated

Instance Method

# start(\_:)

Adds a set of downloads to the download list.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
func start(_ downloads: [SKDownload])
```

Deprecated

Hosted content is no longer supported

## Parameters 

`downloads`  

An array of SKDownload objects to begin downloading.

## Mentioned in 

Unlocking purchased content

## Discussion

In order for a download object to be queued, it must be associated with a transaction that has been successfully purchased, but not yet finished.

## See Also

### Downloading Content

func cancel([SKDownload])

Removes a set of downloads from the download list.

Deprecated

func pause([SKDownload])

Pauses a set of downloads.

Deprecated

func resume([SKDownload])

Resumes a set of downloads.

Deprecated

