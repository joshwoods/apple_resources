

- SwiftUI
- EnvironmentValues
-  disableAutocorrection Deprecated

Instance Property

# disableAutocorrection

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 8.0–11.4Deprecated

``` source
var disableAutocorrection: Bool? { get set }
```

## Discussion

When the value is `nil`, SwiftUI uses the system default. The default value is `nil`.

## See Also

### Deprecated environment values

var sizeCategory: ContentSizeCategory

The size of content.

Deprecated

var presentationMode: Binding&lt;PresentationMode>

A binding to the current presentation mode of the view associated with this environment.

Deprecated

struct PresentationMode

An indication whether a view is currently presented by another view.

Deprecated

var complicationRenderingMode: ComplicationRenderingMode

The complication rendering mode for the current environment.

Deprecated

var controlActiveState: ControlActiveState

The active appearance expected of controls in a window.

Deprecated

