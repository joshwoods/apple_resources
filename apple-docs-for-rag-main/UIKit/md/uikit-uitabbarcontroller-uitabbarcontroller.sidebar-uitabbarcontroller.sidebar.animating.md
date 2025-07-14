

- UIKit
- UITabBarController
- UITabBarController.Sidebar
-  UITabBarController.Sidebar.Animating 

Protocol

# UITabBarController.Sidebar.Animating

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
protocol Animating : NSObjectProtocol
```

## Topics

### Instance Methods

func addAnimations(() -> Void)

**Required**

func addCompletion(() -> Void)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

class UITabSidebarItem

class Request

