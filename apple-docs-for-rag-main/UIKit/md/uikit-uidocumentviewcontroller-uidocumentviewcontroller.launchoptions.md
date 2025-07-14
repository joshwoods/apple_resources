

- UIKit
- UIDocumentViewController
-  UIDocumentViewController.LaunchOptions 

Class

# UIDocumentViewController.LaunchOptions

Options for customizing the document launch view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
class LaunchOptions
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Overview

When your app launches, the document view controller displays a view that contains a title and buttons to create new documents. It also displays the document browser as a sheet over the title view. For more information, see Customizing a document-based app’s launch experience.

## Topics

### Configuring the appearance

var title: String

The title that appears in the title view.

var background: UIBackgroundConfiguration

A configuration that describes the launch scene’s background.

var documentTargetView: UIView?

The document target view.

var browserViewController: UIDocumentBrowserViewController

The document browser view controller.

### Adding accessory views

var backgroundAccessoryView: UIView?

A view that appears behind the title view in the launch scene.

var foregroundAccessoryView: UIView?

A view that appears in front of the title view in the launch scene.

### Adding actions

var primaryAction: UIAction?

The launch scene’s primary action.

var secondaryAction: UIAction?

The launch scene’s secondary action.

### Creating documents

class func createDocumentAction(withIntent: UIDocument.CreationIntent) -> UIAction

Creates an action that uses the specified intent.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Customizing the launch experience

var launchOptions: UIDocumentViewController.LaunchOptions

Options that customize a document-based app’s launch view.

