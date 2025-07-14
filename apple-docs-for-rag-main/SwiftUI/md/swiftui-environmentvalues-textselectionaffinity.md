

- SwiftUI
- EnvironmentValues
-  textSelectionAffinity 

Instance Property

# textSelectionAffinity

A representation of the direction or association of a selection or cursor relative to a text character. This concept becomes much more prominent when dealing with bidirectional text (text that contains both LTR and RTL scripts, like English and Arabic combined).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var textSelectionAffinity: TextSelectionAffinity { get set }
```

## Discussion

You can configure the selection affinity on a given hierarchy by using the textSelectionAffinity(_:) modifier.

## See Also

### Selecting text

func textSelection&lt;S>(S) -> some View

Controls whether people can select text within this view.

protocol TextSelectability

A type that describes the ability to select text.

struct TextSelection

Represents a selection of text.

func textSelectionAffinity(TextSelectionAffinity) -> some View

Sets the direction of a selection or cursor relative to a text character.

enum TextSelectionAffinity

A representation of the direction or association of a selection or cursor relative to a text character. This concept becomes much more prominent when dealing with bidirectional text (text that contains both LTR and RTL scripts, like English and Arabic combined).

