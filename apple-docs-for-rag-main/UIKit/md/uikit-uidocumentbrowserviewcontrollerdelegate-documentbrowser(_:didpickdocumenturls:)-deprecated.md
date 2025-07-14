

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:didPickDocumentURLs:) Deprecated

Instance Method

# documentBrowser(\_:didPickDocumentURLs:)

Tells the delegate that the user has selected one or more documents.

iOS 11.0–12.0DeprecatediPadOS 11.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    didPickDocumentURLs documentURLs: [URL]
)
```

Deprecated

Use documentPicker(_:didPickDocumentsAt:) instead.

## Parameters 

`controller`  

The current document browser.

`documentURLs`  

An array of URLs for the selected documents.

If the document browser’s allowsPickingMultipleItems property is true, the array contains one or more URLs. If false, it contains only a single URL.

## Mentioned in 

Presenting selected documents

## Discussion

Implement this method to process the documents selected by the user. Typically, you create a view controller to display the selected documents, then present that view modally, like in the following example.

```
// Did Select Documents
func documentBrowser(_ controller: UIDocumentBrowserViewController,
                     didPickDocumentURLs documentURLs: [URL]) {

    assert(controller.allowsPickingMultipleItems == false)

    assert(documentURLs.count > 0,
           "*** We received an empty array of documents ***")

    assert(documentURLs.count 

