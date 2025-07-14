

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:didPickDocumentsAt:) 

Instance Method

# documentBrowser(\_:didPickDocumentsAt:)

Tells the delegate that the user has selected one or more documents.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    didPickDocumentsAt documentURLs: [URL]
)
```

## Parameters 

`controller`  

The current document browser.

`documentURLs`  

An array of URLs for the selected documents.

If the document browser’s allowsPickingMultipleItems property is true, the array contains one or more URLs. If false, it contains only a single URL.

## Discussion

Implement this method to process the documents selected by the user. Typically, you create a view controller to display the selected documents, then present that view modally, like in the following code.

```
// Did Select Documents
func documentBrowser(_ controller: UIDocumentBrowserViewController,
    didPickDocumentsAt documentURLs: [URL]) {

    assert(controller.allowsPickingMultipleItems == false)

    assert(documentURLs.count > 0,
           "*** We received an empty array of documents ***")

    assert(documentURLs.count 

