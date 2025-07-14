

- UIKit
- UIDocumentBrowserViewController
-  additionalTrailingNavigationBarButtonItems 

Instance Property

# additionalTrailingNavigationBarButtonItems

Additional bar button items that the document browser displays on the trailing side of its navigation bar.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var additionalTrailingNavigationBarButtonItems: [UIBarButtonItem] { get set }
```

## Mentioned in 

Adding custom actions and activities

## Discussion

Actions triggered by these items don’t have any access to the browser’s content or to the URLs of selected items. Use these bar button items for global actions only (actions that don’t affect a specific document or folder).

Note

Bar button items added using this property don’t appear in Mac apps built with Mac Catalyst. You must find another way to display these actions (for example, using UIMenuBuilder to add the actions to your app’s menu).

## See Also

### Modifying the browser’s appearance

var browserUserInterfaceStyle: UIDocumentBrowserViewController.BrowserUserInterfaceStyle

The visual style for the document browser.

enum BrowserUserInterfaceStyle

Styles that define the document browser’s appearance.

var additionalLeadingNavigationBarButtonItems: [UIBarButtonItem]

Additional bar button items that the document browser displays on the leading side of its navigation bar.

var shouldShowFileExtensions: Bool

A Boolean value that determines whether the browser always shows file extensions.

var localizedCreateDocumentActionTitle: String

The title for the Create Document button.

var defaultDocumentAspectRatio: CGFloat

The aspect ratio for the Create Document button.

