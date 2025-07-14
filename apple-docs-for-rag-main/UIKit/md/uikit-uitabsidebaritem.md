

- UIKit
-  UITabSidebarItem 

Class

# UITabSidebarItem

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
class UITabSidebarItem
```

## Topics

### Classes

class Request

### Initializers

convenience init(request: UITabSidebarItem.Request)

### Instance Properties

var accessories: [UICellAccessory]

var backgroundConfiguration: UIBackgroundConfiguration

var configurationState: UICellConfigurationState

var content: UITabSidebarItem.Content

var contentConfiguration: any UIContentConfiguration

### Instance Methods

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

func defaultContentConfiguration() -> UIListContentConfiguration

### Enumerations

enum Content

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Supporting the sidebar

var mode: UITabBarController.Mode

The display mode for a tab bar.

enum Mode

A tab bar’s display mode.

var sidebar: UITabBarController.Sidebar

A tab bar’s corresponding sidebar.

class Sidebar

An object for managing and configuring the sidebar.

class Request

protocol Animating

