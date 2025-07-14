

- UIKit
- UIDocumentBrowserViewController
-  UIDocumentBrowserViewController.BrowserUserInterfaceStyle 

Enumeration

# UIDocumentBrowserViewController.BrowserUserInterfaceStyle

Styles that define the document browser’s appearance.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
enum BrowserUserInterfaceStyle
```

## Topics

### User interface styles

case dark

A dark background.

case light

A light background.

case white

A white background.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying the browser’s appearance

var browserUserInterfaceStyle: UIDocumentBrowserViewController.BrowserUserInterfaceStyle

The visual style for the document browser.

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

