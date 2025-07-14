

- AppKit
- NSView
-  NSView.DefinitionOptionKey 

Structure

# NSView.DefinitionOptionKey

Keys to include in your definition.

macOS

``` source
struct DefinitionOptionKey
```

## Topics

### Option Key

static let presentationType: NSView.DefinitionOptionKey

An optional key in the options dictionary that specifies the presentation type of the definition display.

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

struct DefinitionPresentationType

Presentation options for the window.

