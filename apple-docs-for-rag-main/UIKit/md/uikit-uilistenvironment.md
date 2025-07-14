

- UIKit
-  UIListEnvironment 

Enumeration

# UIListEnvironment

Constants that indicate the style of the containing list in a collection view or table view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
enum UIListEnvironment
```

## Topics

### Constants

case unspecified

A constant that indicates the absence of information about a containing list.

case none

A constant that indicates there isn’t a containing list.

case plain

A constant that indicates the containing list is a plain-style list.

case grouped

A constant that indicates the containing list is a grouped-style list.

case insetGrouped

A constant that indicates the containing list is an inset-grouped-style list.

case sidebar

A constant that indicates the containing list is a sidebar-style list.

case sidebarPlain

A constant that indicates the containing list is a sidebar-plain-style list.

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

### Retrieving list environment traits

var listEnvironment: UIListEnvironment

