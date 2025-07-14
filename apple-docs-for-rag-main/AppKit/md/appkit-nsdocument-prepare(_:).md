

- AppKit
- NSDocument
-  prepare(\_:) 

Instance Method

# prepare(\_:)

Perform any custom setup associated with a sharing service picker.

macOS 10.13+

``` source
@MainActor
func prepare(_ sharingServicePicker: NSSharingServicePicker)
```

## Parameters 

`sharingServicePicker`  

The sharing service picker the system is about to display.

## Discussion

Override this method, as needed, and use it to configure the sharing service picker before AppKit displays it. The default implementation of this method does nothing. You might customize the contents of the share menu or provide a custom delegate for the chosen sharing service. You can get the default sharing menu item by calling standardShareMenuItem() on the current document controller.

## See Also

### Sharing the Document

var allowsDocumentSharing: Bool

A Boolean value that indicates whether the document is shareable from the standard Share menu.

func share(with: NSSharingService, completionHandler: ((Bool) -> Void)?)

Share the document’s file using the specified sharing service.

