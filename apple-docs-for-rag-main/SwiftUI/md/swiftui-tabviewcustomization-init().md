

- SwiftUI
- TabViewCustomization
-  init() 

Initializer

# init()

Creates an empty tab sidebar customization.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init()
```

## Discussion

To set this customization on a tab view, use the tabViewCustomization(_:) modifier.

With an empty customization, tabs will be visible according to the default builder visibilities, and sections will be ordered in the order declared in the tab view’s tab builder.

You can specify a default visibility for the tab in the tab bar and sidebar by attaching defaultVisibility(_:for:) to the tab.

You can change the default section order by changing the order in the builder. If there’s an existing persisted customization, reset the order by calling resetTabOrder() when you change the order.

