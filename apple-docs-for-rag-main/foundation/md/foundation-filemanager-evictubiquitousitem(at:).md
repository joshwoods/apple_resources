

- Foundation
- FileManager
-  evictUbiquitousItem(at:) 

Instance Method

# evictUbiquitousItem(at:)

Removes the local copy of the specified item that’s stored in iCloud.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func evictUbiquitousItem(at url: URL) throws
```

## Parameters 

`url`  

The URL to a file or directory in iCloud storage.

## Discussion

Don’t use a coordinated write to perform this operation. In macOS 10.7 or earlier, the framework takes a coordinated write in its implementation of this method, so taking one in your app causes a deadlock. In macOS 10.8 and later, the framework detects coordination done by your app on the same thread as the call to this method, to avoid deadlocking.

This method doesn’t remove the item from iCloud. It removes only the local version. You can then use startDownloadingUbiquitousItem(at:) to force iCloud to download a new version of the file or directory from the server.

To delete a file permanently from the user’s iCloud storage, use the regular FileManager routines for deleting files and directories. Remember that deleting items from iCloud can’t be undone. Once deleted, the item is gone forever.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

### Managing iCloud-Based Items

var ubiquityIdentityToken: (any NSCoding &amp; NSCopying &amp; NSObjectProtocol)?

An opaque token that represents the current user’s iCloud Drive Documents identity.

func url(forUbiquityContainerIdentifier: String?) -> URL?

Returns the URL for the iCloud container associated with the specified identifier and establishes access to that container.

func isUbiquitousItem(at: URL) -> Bool

Returns a Boolean indicating whether the item is targeted for storage in iCloud.

func setUbiquitous(Bool, itemAt: URL, destinationURL: URL) throws

Indicates whether the item at the specified URL should be stored in iCloud.

func startDownloadingUbiquitousItem(at: URL) throws

Starts downloading (if necessary) the specified item to the local system.

func url(forPublishingUbiquitousItemAt: URL, expiration: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?) throws -> URL

Returns a URL that can be emailed to users to allow them to download a copy of a flat file item from iCloud.

