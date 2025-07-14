

- UIKit
- UIDocumentBrowserViewController
-  localizedCreateDocumentActionTitle 

Instance Property

# localizedCreateDocumentActionTitle

The title for the Create Document button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localizedCreateDocumentActionTitle: String { get set }
```

## Discussion

The default value is `Create Document`.

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

var defaultDocumentAspectRatio: CGFloat

The aspect ratio for the Create Document button.

