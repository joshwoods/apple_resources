

- AppKit
- NSDocument
-  usesUbiquitousStorage 

Type Property

# usesUbiquitousStorage

Returns whether the document object stores its contents in the user’s iCloud document storage.

macOS 10.8+

``` source
@MainActor
class var usesUbiquitousStorage: Bool { get }
```

## Discussion

This method’s default implementation returns true if your app has a valid iCloud document storage entitlement (`com.apple.developer.ubiquity-container-identifiers` or `com.apple.developer.icloud-container-identifiers`, as described in Entitlement Key Reference). When this method returns true, the system adds new menu items and other UI for iCloud documents, as appropriate, and allows documents to be saved or moved into the primary iCloud container. (The primary iCloud container is the one identified by the first container identifier string in the iCloud Containers list in the Xcode target editor.)

To indicate that your NSDocument subclass does not use iCloud storage, override this method to return false.

## See Also

### Storing Documents in iCloud

func moveToUbiquityContainer(Any?)

Moves the document to the user’s iCloud storage.

