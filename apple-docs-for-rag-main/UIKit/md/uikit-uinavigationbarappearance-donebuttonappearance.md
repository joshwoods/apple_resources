

- UIKit
- UINavigationBarAppearance
-  doneButtonAppearance 

Instance Property

# doneButtonAppearance

The appearance attributes for Done buttons.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var doneButtonAppearance: UIBarButtonItemAppearance { get set }
```

## Discussion

Use this property to configure the appearance of bar button items that use the UIBarButtonItem.Style.done style, when appropriate. If the navigation bar doesn’t have a done button, setting the value of this property has no effect.

