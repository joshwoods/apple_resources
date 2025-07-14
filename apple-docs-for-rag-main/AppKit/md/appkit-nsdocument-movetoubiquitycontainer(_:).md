

- AppKit
- NSDocument
-  moveToUbiquityContainer(\_:) 

Instance Method

# moveToUbiquityContainer(\_:)

Moves the document to the user’s iCloud storage.

macOS 10.8+

``` source
@IBAction @MainActor
func moveToUbiquityContainer(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

AppKit calls this method automatically in response to the user selecting the Move to iCloud… menu item in a document-based app. The default implementation presents the user with an alert asking to confirm the move before invoking the move(to:completionHandler:) method with a URL in the app’s default ubiquity container.

See Moving the Document for descriptions of methods for moving a document to a local path.

## See Also

### Storing Documents in iCloud

class var usesUbiquitousStorage: Bool

Returns whether the document object stores its contents in the user’s iCloud document storage.

