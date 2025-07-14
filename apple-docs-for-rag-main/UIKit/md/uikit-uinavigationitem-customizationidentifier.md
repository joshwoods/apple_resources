

- UIKit
- UINavigationItem
-  customizationIdentifier 

Instance Property

# customizationIdentifier

A globally unique string that enables user customization of the navigation bar layout.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var customizationIdentifier: String? { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Set a customization identifier to support a personalized navigation bar layout experience. When you assign a string to this property, UIKit allows people to customize the layout of the items in the navigation bar by choosing the customize option in the overflow menu. UIKit automatically saves and restores this custom layout across app launches.

