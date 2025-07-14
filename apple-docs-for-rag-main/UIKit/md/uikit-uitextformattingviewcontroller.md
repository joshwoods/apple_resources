

- UIKit
-  UITextFormattingViewController 

Class

# UITextFormattingViewController

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
class UITextFormattingViewController
```

## Topics

### Classes

class Component

class ComponentGroup

class Configuration

### Global variables

static let fontAttributes: UITextFormattingViewController.ComponentKey

static let fontPicker: UITextFormattingViewController.ComponentKey

static let fontPointSize: UITextFormattingViewController.ComponentKey

static let fontSize: UITextFormattingViewController.ComponentKey

static let formattingStyles: UITextFormattingViewController.ComponentKey

static let highlight: UITextFormattingViewController.ComponentKey

static let highlightPicker: UITextFormattingViewController.ComponentKey

static let lineHeight: UITextFormattingViewController.ComponentKey

static let listStyles: UITextFormattingViewController.ComponentKey

static let textAlignment: UITextFormattingViewController.ComponentKey

static let textAlignmentAndJustification: UITextFormattingViewController.ComponentKey

static let textColor: UITextFormattingViewController.ComponentKey

static let textIndentation: UITextFormattingViewController.ComponentKey

static let blue: UITextFormattingViewController.Highlight

static let `default`: UITextFormattingViewController.Highlight

static let mint: UITextFormattingViewController.Highlight

static let orange: UITextFormattingViewController.Highlight

static let pink: UITextFormattingViewController.Highlight

static let purple: UITextFormattingViewController.Highlight

static let center: UITextFormattingViewController.TextAlignment

static let justified: UITextFormattingViewController.TextAlignment

static let left: UITextFormattingViewController.TextAlignment

static let natural: UITextFormattingViewController.TextAlignment

static let right: UITextFormattingViewController.TextAlignment

static let decimal: UITextFormattingViewController.TextList

static let disc: UITextFormattingViewController.TextList

static let hyphen: UITextFormattingViewController.TextList

static let other: UITextFormattingViewController.TextList

### Protocols

protocol Delegate

### Structures

struct FormattingDescriptor

struct FormattingStyle

### Initializers

init()

init(configuration: UITextFormattingViewController.Configuration)

### Instance Properties

var configuration: UITextFormattingViewController.Configuration

var delegate: (any UITextFormattingViewController.Delegate)?

var formattingDescriptor: UITextFormattingViewController.FormattingDescriptor?

### Enumerations

enum ChangeValue

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

