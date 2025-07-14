

- UIKit
- UIDocument
-  fileModificationDate 

Instance Property

# fileModificationDate

The date and time your app last modified the document file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var fileModificationDate: Date? { get set }
```

## Discussion

The modification date is updated by the open(completionHandler:), save(to:for:completionHandler:), and revert(toContentsOf:completionHandler:) methods. Its value is `nil` if none of these methods has completed successfully at least once. If you override any of these methods, you should be sure to set this property in your implementation.

UIKit sets this property before it calls the completion handlers of the open(completionHandler:), save(to:for:completionHandler:), and revert(toContentsOf:completionHandler:). If, outside of these methods or their completion handlers, you want to wait for any pending file operations to complete before you access this property, you can call performAsynchronousFileAccess(_:) and access the property value in the block parameter.

Important

This API has the potential of being misused to access device signals to try to identify the device or user, also known as fingerprinting. Regardless of whether a user gives your app permission to track, fingerprinting is not allowed. When you use this API in your app or third-party SDK (an SDK not provided by Apple), declare your usage and the reason for using the API in your app or third-party SDK’s `PrivacyInfo.xcprivacy` file. For more information, including the list of valid reasons for using the API, see Describing use of required reason API.

## See Also

### Accessing document attributes

var fileURL: URL

The file URL you use to initialize the document.

var localizedName: String

The localized name of the document.

var fileType: String?

The file type of the document.

var documentState: UIDocument.State

The current state of the document.

var progress: Progress?

The upload or download progress of a document.

