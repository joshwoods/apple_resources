

- SwiftUI
- CustomizableToolbarContent
-  defaultCustomization(\_:options:) 

Instance Method

# defaultCustomization(\_:options:)

Configures the way customizable toolbar items with the default behavior behave.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func defaultCustomization(
    _ defaultVisibility: Visibility = .automatic,
    options: ToolbarCustomizationOptions = []
) -> some CustomizableToolbarContent
```

## Parameters 

`defaultVisibility`  

The default visibility of toolbar content with the default customization behavior.

`options`  

The customization options to configure the behavior of toolbar content with the default customization behavior.

## Discussion

Default customizable items support a variety of edits by the user.

- A user can add an an item that is not in the toolbar.

- A user can remove an item that is in the toolbar.

- A user can move an item within the toolbar.

By default, all default customizable items will be initially present in the toolbar. Provide a value of Visibility.hidden to this modifier to specify that items should initially be hidden from the user, and require them to add those items to the toolbar if desired.

```
ContentView()
    .toolbar(id: "main") {
        ToolbarItem(id: "new") {
            // new button here
        }
        .defaultCustomization(.hidden)
    }
```

You can ensure that the user can always use an item with default customizability, even if it’s removed from the customizable toolbar. To do this, provide the alwaysAvailable option. These items will remain in the overflow if the user removes them from the toolbar.

Provide a value of alwaysAvailable to the options parameter of this modifier to receive this behavior.

```
ContentView()
    .toolbar(id: "main") {
        ToolbarItem(id: "new") {
            // new button here
        }
        .defaultCustomization(options: .alwaysAvailable)
    }
```

## See Also

### Using default options

func defaultCustomization() -> some CustomizableToolbarContent

Configures customizable toolbar content with the default visibility and options.

Deprecated

