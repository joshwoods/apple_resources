

- UIKit
- UIDocumentBrowserViewController
-  defaultDocumentAspectRatio 

Instance Property

# defaultDocumentAspectRatio

The aspect ratio for the Create Document button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var defaultDocumentAspectRatio: CGFloat { get set }
```

## Discussion

The aspect ratio is defined as the button’s width divided by its height. The default is `2.0/3.0`.

## See Also

### Modifying the browser’s appearance

var browserUserInterfaceStyle: UIDocumentBrowserViewController.BrowserUserInterfaceStyle

The visual style for the document browser.

enum BrowserUserInterfaceStyle

Styles that define the document browser’s appearance.

var additionalLeadingNavigationBarButtonItems: [UIBarButtonItem]

Additional bar button items that the document browser displays on the leading side of its navigation bar.

var additionalTrailingNavigationBarButtonItems: [UIBarButtonItem]

Additional bar button items that the document browser displays on the trailing side of its navigation bar.

var shouldShowFileExtensions: Bool

A Boolean value that determines whether the browser always shows file extensions.

var localizedCreateDocumentActionTitle: String

The title for the Create Document button.

