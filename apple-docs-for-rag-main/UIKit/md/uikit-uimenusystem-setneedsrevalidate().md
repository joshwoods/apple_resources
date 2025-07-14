

- UIKit
- UIMenuSystem
-  setNeedsRevalidate() 

Instance Method

# setNeedsRevalidate()

Tells the menu system to validate all of its menus.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setNeedsRevalidate()
```

## Discussion

Call this method when your app needs to revalidate a menu, such as when the state of your app changes.

