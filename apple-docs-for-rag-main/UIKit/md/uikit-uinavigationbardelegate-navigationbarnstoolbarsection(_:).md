

- UIKit
- UINavigationBarDelegate
-  navigationBarNSToolbarSection(\_:) 

Instance Method

# navigationBarNSToolbarSection(\_:)

Asks the delegate which section of the toolbar to host the navigation bar in.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func navigationBarNSToolbarSection(_ navigationBar: UINavigationBar) -> UINavigationBar.NSToolbarSection
```

## Parameters 

`navigationBar`  

The navigation bar to host in an NSToolbar.

## Return Value

An NSToolbar section that determines which section to place the navigation bar in, and how to present the navigation bar in that section. Return UINavigationBar.NSToolbarSection.none to disable NSToolbar hosting, which is equivalent to setting preferredBehavioralStyle to UIBehavioralStyle.pad.

## Discussion

The system calls this method to determine how to render your UINavigationBar when you build your app with Mac Catalyst.

