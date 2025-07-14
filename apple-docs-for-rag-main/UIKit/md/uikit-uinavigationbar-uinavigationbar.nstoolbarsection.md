

- UIKit
- UINavigationBar
-  UINavigationBar.NSToolbarSection 

Enumeration

# UINavigationBar.NSToolbarSection

Constants that determine how the system hosts the navigation bar in an AppKit toolbar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum NSToolbarSection
```

## Topics

### Constants

case none

A constant that disables hosting the navigation bar in the toolbar.

case sidebar

A constant that hosts the navigation bar in the toolbar’s sidebar column.

case supplementary

A constant that hosts the navigation bar in the toolbar’s supplementary column.

case content

A constant that hosts the navigation bar in the toolbar’s content column.

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

### Building with Mac Catalyst

var behavioralStyle: UIBehavioralStyle

The behavioral style of the navigation bar.

var preferredBehavioralStyle: UIBehavioralStyle

The preferred behavioral style of the navigation bar.

var currentNSToolbarSection: UINavigationBar.NSToolbarSection

The toolbar section that the navigation bar is currently using.

