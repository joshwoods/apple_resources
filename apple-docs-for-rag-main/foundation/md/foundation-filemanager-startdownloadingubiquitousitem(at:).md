

- Foundation
- FileManager
-  startDownloadingUbiquitousItem(at:) 

Instance Method

# startDownloadingUbiquitousItem(at:)

Starts downloading (if necessary) the specified item to the local system.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func startDownloadingUbiquitousItem(at url: URL) throws
```

## Parameters 

`url`  

The URL for the file or directory in the cloud that you want to download.

## Discussion

If a cloud-based file or directory has not been downloaded yet, calling this method starts the download process. If the item exists locally, calling this method synchronizes the local copy with the version in the cloud.

For a given URL, you can determine if a file is downloaded by getting the value of the NSMetadataUbiquitousItemDownloadingStatusKey key. You can also use related keys to determine the current progress in downloading the file.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing iCloud-Based Items

var ubiquityIdentityToken: (any NSCoding &amp; NSCopying &amp; NSObjectProtocol)?

An opaque token that represents the current user’s iCloud Drive Documents identity.

func url(forUbiquityContainerIdentifier: String?) -> URL?

Returns the URL for the iCloud container associated with the specified identifier and establishes access to that container.

func isUbiquitousItem(at: URL) -> Bool

Returns a Boolean indicating whether the item is targeted for storage in iCloud.

func setUbiquitous(Bool, itemAt: URL, destinationURL: URL) throws

Indicates whether the item at the specified URL should be stored in iCloud.

func evictUbiquitousItem(at: URL) throws

Removes the local copy of the specified item that’s stored in iCloud.

func url(forPublishingUbiquitousItemAt: URL, expiration: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?) throws -> URL

Returns a URL that can be emailed to users to allow them to download a copy of a flat file item from iCloud.

