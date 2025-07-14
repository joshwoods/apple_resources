

- UIKit
- UIDocumentBrowserAction
-  UIDocumentBrowserAction.Availability 

Structure

# UIDocumentBrowserAction.Availability

Values that determine where the action can appear in the document browser.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct Availability
```

## Topics

### Constants

static var menu: UIDocumentBrowserAction.Availability

An action that appears in the Edit Menu when the user long presses a supported document.

static var navigationBar: UIDocumentBrowserAction.Availability

An action that appears in the navigation bar when the user puts the document browser in Select mode.

### Initializers

init(rawValue: Int)

Returns a newly instantiated availability instance.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing activity data

var identifier: String

The action’s unique identifier.

var localizedTitle: String

The title that appears in the menu or navigation bar.

var availability: UIDocumentBrowserAction.Availability

A value that defines where the action can appear (in the Edit Menu, the navigation bar, or both).

