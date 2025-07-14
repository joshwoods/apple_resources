

- AppKit
- NSDocument
-  share(with:completionHandler:) 

Instance Method

# share(with:completionHandler:)

Share the document’s file using the specified sharing service.

macOS 10.13+

``` source
@MainActor
func share(
    with sharingService: NSSharingService,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
@MainActor
func share(with sharingService: NSSharingService) async -> Bool
```

## Parameters 

`sharingService`  

The sharing service that is sharing the document.

`completionHandler`  

The completion handler block to call with the results. AppKit calls this method after attempting to share the document. The handler block has no return value and takes the following parameter:

success  
A Boolean value indicating whether the sharing attempt was successful. The value is true if sharing succeeded, or false if it didn’t.

## Discussion

This method shares the document’s file, located at fileURL, with the specified sharing service. If the document has never been saved, this method prompts the user to save it before proceeding; otherwise, the method initiates an autosave operation to save any outstanding changes. As needed, the method moves the file to an appropriate location for sharing. For example, when saving to iCloud, the method moves the file to the user’s iCloud Drive folder. After the sharing service finishes, the method calls `completionHandler` with the results.

The document temporarily replaces the current delegate of `sharingService` with itself. However, the document retains a reference to the old delegate object and forwards all delegate method calls to it.

If an NSDocument object is the only item associated with an NSSharingServicePicker or NSSharingServicePickerTouchBarItem, the picker automatically calls this method directly, instead of sharing the items using the perform(withItems:) method.

If you override this method, you must ensure that the document is in the proper state before attempting to share it. For example, you are responsible for ensuring the file is in an appropriate location. When your sharing service finishes, you must execute the provided `completionHandler` block with the results.

## See Also

### Sharing the Document

var allowsDocumentSharing: Bool

A Boolean value that indicates whether the document is shareable from the standard Share menu.

func prepare(NSSharingServicePicker)

Perform any custom setup associated with a sharing service picker.

