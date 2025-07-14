

- UIKit
- UIDocumentViewController
- UIDocumentViewController.LaunchOptions
-  createDocumentAction(withIntent:) 

Type Method

# createDocumentAction(withIntent:)

Creates an action that uses the specified intent.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
class func createDocumentAction(withIntent intent: UIDocument.CreationIntent) -> UIAction
```

## Parameters 

`intent`  

An intent that defines how your app creates the document.

## Mentioned in 

Customizing a document-based app’s launch experience

## Discussion

Use this method to create an action that you can assign to your primaryAction or secondaryAction. When the system triggers the action, it calls your UIDocumentBrowserViewControllerDelegate object’s documentBrowser(_:didRequestDocumentCreationWithHandler:) method. For more information, see Customizing a document-based app’s launch experience.

