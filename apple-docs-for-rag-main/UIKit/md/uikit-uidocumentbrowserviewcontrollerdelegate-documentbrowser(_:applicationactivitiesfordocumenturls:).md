

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:applicationActivitiesForDocumentURLs:) 

Instance Method

# documentBrowser(\_:applicationActivitiesForDocumentURLs:)

Asks the delegate for additional activities when displaying an activity view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    applicationActivitiesForDocumentURLs documentURLs: [URL]
) -> [UIActivity]
```

## Parameters 

`controller`  

The current document browser.

`documentURLs`  

The URL of one or more documents to share.

## Return Value

An array of custom UIActivity objects.

## Mentioned in 

Adding custom actions and activities

## Discussion

The document browser displays an activity view when the user shares a document (for example, when the user long presses a document and then chooses Share from the Edit Menu).

Implement this method to add custom activities to the activity view. Create and return an array containing your custom UIActivity subclasses. Your UIActivity subclasses should perform actions on the URLs passed to this method.

Note

Do not assume that the URL array contains only one URL. The user can place the document browser into Select mode and select multiple documents to share, even if the document browser’s allowsPickingMultipleItems property is false.

## See Also

### Working with the browser’s activity view

func documentBrowser(UIDocumentBrowserViewController, willPresent: UIActivityViewController)

Tells the delegate that the document browser will display an activity view.

