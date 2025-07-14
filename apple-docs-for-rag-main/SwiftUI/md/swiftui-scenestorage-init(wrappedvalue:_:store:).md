

- SwiftUI
- SceneStorage
-  init(wrappedValue:\_:store:) 

Initializer

# init(wrappedValue:\_:store:)

Creates a property that can save and restore tab sidebar customizations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    wrappedValue: Value = TabViewCustomization(),
    _ key: String,
    store: UserDefaults? = nil
) where Value == TabViewCustomization
```

## Parameters 

`wrappedValue`  

The default value if the customization is not available for the given key.

`key`  

A key used to save and restore the value.

## Discussion

You can set this customization on the TabView using tabViewCustomization(_:).

The tab view customization is typically not added to `SceneStorage`, but instead stored in `AppStorage` so the customizations are consistent across different scenes.

