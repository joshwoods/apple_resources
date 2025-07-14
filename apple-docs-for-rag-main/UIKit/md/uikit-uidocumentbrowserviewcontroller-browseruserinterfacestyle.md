

- UIKit
- UIDocumentBrowserViewController
-  browserUserInterfaceStyle 

Instance Property

# browserUserInterfaceStyle

The visual style for the document browser.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
var browserUserInterfaceStyle: UIDocumentBrowserViewController.BrowserUserInterfaceStyle { get set }
```

## Mentioned in 

Customizing the browser

## Discussion

For a list of possible styles, see UIDocumentBrowserViewController.BrowserUserInterfaceStyle.

Note

This property has no effect in Mac apps built with Mac Catalyst.

## See Also

### Modifying the browser’s appearance

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

var defaultDocumentAspectRatio: CGFloat

The aspect ratio for the Create Document button.

