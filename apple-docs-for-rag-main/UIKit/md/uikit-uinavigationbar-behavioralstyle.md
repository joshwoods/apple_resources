

- UIKit
- UINavigationBar
-  behavioralStyle 

Instance Property

# behavioralStyle

The behavioral style of the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var behavioralStyle: UIBehavioralStyle { get }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Use this property to determine the actual behavior style when the preferredBehavioralStyle is UIBehavioralStyle.automatic.

When the value of this property is UIBehavioralStyle.mac, NSToolbar hosts the navigation bar’s content when you build your app with Mac Catalyst.

## See Also

### Building with Mac Catalyst

var preferredBehavioralStyle: UIBehavioralStyle

The preferred behavioral style of the navigation bar.

var currentNSToolbarSection: UINavigationBar.NSToolbarSection

The toolbar section that the navigation bar is currently using.

enum NSToolbarSection

Constants that determine how the system hosts the navigation bar in an AppKit toolbar.

