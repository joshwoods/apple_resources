

- SwiftUI
-  ListSectionSpacing 

Structure

# ListSectionSpacing

The spacing options between two adjacent sections in a list.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ListSectionSpacing
```

## Topics

### Getting section spacing

static let `default`: ListSectionSpacing

The default spacing between sections

static let compact: ListSectionSpacing

Compact spacing between sections

static func custom(CGFloat) -> ListSectionSpacing

Creates a custom spacing value.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring spacing

func listRowSpacing(CGFloat?) -> some View

Sets the vertical spacing between two adjacent rows in a List.

func listSectionSpacing(_:)

Sets the spacing between adjacent sections in a List to a custom value.

