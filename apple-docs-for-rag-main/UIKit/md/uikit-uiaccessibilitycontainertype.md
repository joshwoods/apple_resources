

- UIKit
-  UIAccessibilityContainerType 

Enumeration

# UIAccessibilityContainerType

Constants that indicate the type of content in a data-based container.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum UIAccessibilityContainerType
```

## Topics

### Constants

case none

No additional data.

case dataTable

A table that contains structured data.

case list

A list of data.

case landmark

Landmark data.

case semanticGroup

A semantic group of data.

### Useful links

Accessibility design for Mac Catalyst

Improve navigation in your app by using keyboard shortcuts and accessibility containers.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Containers

protocol UIAccessibilityContainerDataTable

Methods that convey information about the contents of a table.

protocol UIAccessibilityContainerDataTableCell

Methods that provide the location of a cell in a table.

