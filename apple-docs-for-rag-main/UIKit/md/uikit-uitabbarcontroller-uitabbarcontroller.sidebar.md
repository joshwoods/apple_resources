

- UIKit
- UITabBarController
-  UITabBarController.Sidebar 

Class

# UITabBarController.Sidebar

An object for managing and configuring the sidebar.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
class Sidebar
```

## Topics

### Setting the sidebar delegate

var delegate: (any UITabBarController.Sidebar.Delegate)?

protocol Delegate

### Scrolling

func scroll(to: UITabBarController.Sidebar.ScrollTarget, animated: Bool)

enum ScrollTarget

### Managing customization

var isHidden: Bool

var preferredLayout: UITabBarController.Sidebar.Layout

enum Layout

func reconfigureItem(for: UITab)

### Headers and footers

var bottomBarView: UIView?

var footerContentConfiguration: (any UIContentConfiguration)?

var headerContentConfiguration: (any UIContentConfiguration)?

### Instance Properties

var navigationOverflowItems: UIDeferredMenuElement?

Additional items to add to the overflow menu in the sidebar’s navigation bar. Setting this property to a non-nil value will force the overflow button to appear, regardless of if you provide any content in the element’s callback. Items returned are displayed directly in the presented menu. When set, the “Edit Sidebar” action will also be moved into the overflow menu after the app-provided items.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

class UITabSidebarItem

class Request

protocol Animating

