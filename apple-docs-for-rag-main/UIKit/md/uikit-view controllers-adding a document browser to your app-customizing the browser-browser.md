

- UIKit
- View controllers
- Adding a document browser to your app
-  Customizing the browser 

Article

# Customizing the browser

Customize the document browser’s look and behavior.

## Overview

You can set the browser’s appearance, create document thumbnails, and modify the browser’s behavior.

### Set the browser’s appearance

Change the browser’s appearance by setting the browserUserInterfaceStyle property. The document browser view controller supports white, light, and dark appearances.

### Create document thumbnails or icons

The system automatically provides thumbnails or icons for supported document types. If your app uses a custom or third-party document type, you can create a Thumbnail extension for that type. For more information, see QLThumbnailProvider.

If you don’t provide a Thumbnail extension, the system can create a document icon based on your app icon. To enable automatic icon creation, go to the Project navigator, choose the target, click Info, and then do the following:

1.  Declare support for the document’s UTI in the Document Type section.

2.  For any custom document types that you create, export the UTI in the Exported UTIs section.

3.  For any third-party document types used by your app, import the UTI in the Imported UTIs section.

For more information, see Set the supported document types.

Your app’s icon only appears in the Files app or document browser when the following are all true:

- The system doesn’t automatically provide a thumbnail for the UTI.

- The system doesn’t already provide an icon for the UTI.

- The user hasn’t installed a Thumbnail extension for the UTI.

- Your app both declares document type support for the UTI and declares the UTI as an exported or imported type.

### Add document previews

The system automatically provides previews for supported document types. If your app uses a custom or third-party document type, you can create a Preview extension for that type.

For more information, see Quick Look.

### Modify the browser’s behavior

You can control the following behaviors:

- The type of documents the browser opens

- Whether the browser opens multiple files at the same time

- Whether the browser creates new documents

#### Set allowed document types

You set the list of allowed document types when you create the browser. Pass an array of uniform type identifier (UTI) strings to the UIDocumentBrowserViewController class’s init(forOpeningFilesWithContentTypes:) method. If you pass `nil`, the browser uses the document types specified by the CFBundleDocumentTypes key in the app’s `Info.plist` file.

For detailed instructions on setting the CFBundleDocumentTypes key, see Set the supported document types).

The following example programmatically creates a document browser for `.txt` files:

```
let browser = UIDocumentBrowserViewController(forOpeningFilesWithContentTypes: ["public.plain-text"])
```

#### Enable multiple document selection

By default, users can select only one item at a time. To enable multiple document selection, set the document browser’s allowsPickingMultipleItems property to true.

#### Enable new document creation

To let users create new documents, you must do the following:

- Set the browser’s allowsDocumentCreation property to true (the default value).

- Implement the UIDocumentBrowserViewControllerDelegate object’s documentBrowser(_:didRequestDocumentCreationWithHandler:) method.

After these steps are completed, the system automatically includes an Add button (+) in the document browser’s navigation bar.

When the user taps the Add button, the system calls the documentBrowser(_:didRequestDocumentCreationWithHandler:) method. In your implementation, you can present a custom user interface, where users can configure the document. For example, you might show a list of document templates.

Create a new document and save it to a temporary location. As soon as the document is saved, call the provided `importHandler`. To confirm the request, pass in the document’s temporary URL and the import mode (UIDocumentBrowserViewController.ImportMode.copy or UIDocumentBrowserViewController.ImportMode.move). To cancel the request, pass `nil` and UIDocumentBrowserViewController.ImportMode.none.

Important

You must always call the `importHandler`. If you can’t create a new document, pass `nil` for the URL and UIDocumentBrowserViewController.ImportMode.none for the import mode.

## See Also

### Customization

Adding custom actions and activities

Add custom document browser actions, activities, and bar items.

