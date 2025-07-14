

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:willPresent:) 

Instance Method

# documentBrowser(\_:willPresent:)

Tells the delegate that the document browser will display an activity view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    willPresent activityViewController: UIActivityViewController
)
```

## Parameters 

`controller`  

The current document browser.

`activityViewController`  

The activity view controller to be displayed.

## Discussion

The document browser displays an activity view when the user shares a document (for example, when the user long presses a document and then chooses Share from the Edit Menu).

Implement this method to customize the activity view before it is displayed. For example, you could exclude any system-provided activities that are inappropriate for your app (see the UIActivityViewController class’s excludedActivityTypes property).

## See Also

### Working with the browser’s activity view

func documentBrowser(UIDocumentBrowserViewController, applicationActivitiesForDocumentURLs: [URL]) -> [UIActivity]

Asks the delegate for additional activities when displaying an activity view.

