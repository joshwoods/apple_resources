

- Safari Services
- SFSafariApplication
-  setToolbarItemsNeedUpdate() 

Type Method

# setToolbarItemsNeedUpdate()

Updates the enabled states and badges of toolbar items.

macOS 10.12+

``` source
class func setToolbarItemsNeedUpdate()
```

## Discussion

This method calls the validateToolbarItem(in:validationHandler:) method on the extension’s principal object for each open window. See SFSafariExtensionHandling.

