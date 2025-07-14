

- StoreKit
-  SKDownload Deprecated

Class

# SKDownload

Downloadable content associated with a product.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
class SKDownload
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Overview

When you create a product in App Store Connect, you can associate one or more pieces of downloadable content with it. At runtime, when a product is purchased by a user, your app uses SKDownload objects to download the content from the App Store.

Your app never directly creates a SKDownload object. Instead, after a payment is processed, your app reads the transaction object’s downloads property to retrieve an array of SKDownload objects associated with the transaction.

To download the content, you queue a download object on the payment queue and wait for the content to be downloaded. After a download completes, read the download object’s contentURL property to get a URL to the downloaded content. Your app must process the downloaded file before completing the transaction. For example, it might copy the file into a directory whose contents are persistent. When all downloads are complete, you finish the transaction. After the transaction is finished, the download objects cannot be queued to the payment queue and any URLs to the downloaded content are invalid.

## Topics

### Getting Content Information

var expectedContentLength: Int64

The length of the downloadable content, in bytes.

var contentIdentifier: String

A string that uniquely identifies the downloadable content.

var contentVersion: String

A string that identifies which version of the content is available for download.

var transaction: SKPaymentTransaction

The transaction associated with the downloadable file.

var contentLength: Int64

The length of the downloadable content, in bytes.

### Getting State Information

var state: SKDownloadState

The current state of the download object.

var progress: Float

A value that indicates how much of the file has been downloaded.

var timeRemaining: TimeInterval

An estimated time, in seconds, to finish downloading the content.

var SKDownloadTimeRemainingUnknown: TimeInterval

Indicates that the system cannot determine how much time is needed to finish downloading the content.

enum SKDownloadState

The states that a download operation can be in.

var downloadState: SKDownloadState

The current state of the download object.

### Accessing a Completed Download

var error: (any Error)?

The error that prevented the content from being downloaded.

var contentURL: URL?

The local location of the downloaded file.

### Managing Downloaded Content

class func contentURL(forProductID: String) -> URL?

Returns the local location for the previously downloaded flie.

class func deleteContent(forProductID: String)

Deletes the previously downloaded file.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Content delivery

Unlocking purchased content

Deliver content to the customer after validating the purchase.

Persisting a purchase

Keep a persistent record of a purchase to continue making the product available as needed.

Finishing a transaction

Finish the transaction to complete the purchase process.

