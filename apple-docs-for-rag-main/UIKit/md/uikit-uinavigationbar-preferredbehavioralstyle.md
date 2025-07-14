

- UIKit
- UINavigationBar
-  preferredBehavioralStyle 

Instance Property

# preferredBehavioralStyle

The preferred behavioral style of the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var preferredBehavioralStyle: UIBehavioralStyle { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Use this property to specify the behavioral style for the navigation bar. If the value of the property is UIBehavioralStyle.automatic, use the behavioralStyle property to determine the actual style.

The default value of this property is UIBehavioralStyle.automatic. To learn more about behavioral styles, see UIBehavioralStyle.

## See Also

### Building with Mac Catalyst

var behavioralStyle: UIBehavioralStyle

The behavioral style of the navigation bar.

var currentNSToolbarSection: UINavigationBar.NSToolbarSection

The toolbar section that the navigation bar is currently using.

enum NSToolbarSection

Constants that determine how the system hosts the navigation bar in an AppKit toolbar.

