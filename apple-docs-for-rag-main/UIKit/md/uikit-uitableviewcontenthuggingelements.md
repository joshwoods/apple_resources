

- UIKit
-  UITableViewContentHuggingElements 

Structure

# UITableViewContentHuggingElements

Constants that determine which types of items in a table view tightly hug their content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
struct UITableViewContentHuggingElements
```

## Topics

### Specifying content-hugging elements

static var sectionHeaders: UITableViewContentHuggingElements

A mode where section headers in the table view tightly hug their content.

### Creating a content-hugging elements structure

init(rawValue: Int)

Creates a content-hugging elements structure.

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

### Managing content-hugging behavior

var contentHuggingElements: UITableViewContentHuggingElements

A setting that determines which type of items tightly hug their content.

