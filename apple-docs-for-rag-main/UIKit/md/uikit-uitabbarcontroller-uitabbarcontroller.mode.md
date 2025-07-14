

- UIKit
- UITabBarController
-  UITabBarController.Mode 

Enumeration

# UITabBarController.Mode

A tab bar’s display mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
enum Mode
```

## Topics

### Setting modes

case automatic

The system sets the display mode based on the tab’s content.

case tabBar

The system displays the content only as a tab bar.

case tabSidebar

The system displays the content as either a tab bar or a sidebar, depending on the context.

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

### Supporting the sidebar

var mode: UITabBarController.Mode

The display mode for a tab bar.

var sidebar: UITabBarController.Sidebar

A tab bar’s corresponding sidebar.

class Sidebar

An object for managing and configuring the sidebar.

class UITabSidebarItem

class Request

protocol Animating

