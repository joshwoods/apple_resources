

- AppKit
- NSView
-  NSView.DefinitionPresentationType 

Structure

# NSView.DefinitionPresentationType

Presentation options for the window.

macOS

``` source
struct DefinitionPresentationType
```

## Topics

### Presentation Values

static let dictionaryApplication: NSView.DefinitionPresentationType

A possible value of the presentationType dictionary key that invokes Dictionary application to display the definition.

static let overlay: NSView.DefinitionPresentationType

A possible value of the presentationType dictionary key that produces a small overlay window at the string location,

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Displaying Definition Windows

func showDefinition(for: NSAttributedString?, at: NSPoint)

Shows a window displaying the definition of the attributed string at the specified point.

func showDefinition(for: NSAttributedString?, range: NSRange, options: [NSView.DefinitionOptionKey : Any]?, baselineOriginProvider: ((NSRange) -> NSPoint)?)

Shows a window displaying the definition of the specified range of the attributed string.

struct DefinitionOptionKey

Keys to include in your definition.

