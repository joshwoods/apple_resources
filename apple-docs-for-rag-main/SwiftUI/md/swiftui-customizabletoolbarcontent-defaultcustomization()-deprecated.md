

- SwiftUI
- CustomizableToolbarContent
-  defaultCustomization() Deprecated

Instance Method

# defaultCustomization()

Configures customizable toolbar content with the default visibility and options.

iOS 16.0–16.0DeprecatediPadOS 16.0–16.0DeprecatedMac Catalyst 16.0–16.0DeprecatedmacOS 13.0–13.0DeprecatedtvOS 16.0–16.0DeprecatedvisionOS 1.0+watchOS 9.0–9.0Deprecated

``` source
func defaultCustomization() -> some CustomizableToolbarContent
```

Deprecated

Please provide either a visibility or customization options

## Discussion

Use the defaultCustomization(_:options:) modifier providing either a `defaultVisibility` or `options` instead.

## See Also

### Using default options

func defaultCustomization(Visibility, options: ToolbarCustomizationOptions) -> some CustomizableToolbarContent

Configures the way customizable toolbar items with the default behavior behave.

