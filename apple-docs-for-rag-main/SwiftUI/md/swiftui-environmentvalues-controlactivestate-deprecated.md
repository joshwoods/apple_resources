

- SwiftUI
- EnvironmentValues
-  controlActiveState Deprecated

Instance Property

# controlActiveState

The active appearance expected of controls in a window.

macOS 10.15–15.4Deprecated

``` source
var controlActiveState: ControlActiveState { get set }
```

Deprecated

Use \`EnvironmentValues.appearsActive\` instead.

## Discussion

`ControlActiveState` and `EnvironmentValues.controlActiveState` are deprecated, use `EnvironmentValues.appearsActive` instead.

Starting with macOS 15.0, the value of this environment property is strictly mapped to and from `EnvironmentValues.appearsActive` as follows:

- `appearsActive == true`, `controlActiveState` returns `.key`

- `appearsActive == false`, `controlActiveState` returns `.inactive`

- `controlActiveState` is set to `.key` or `.active`, `appearsActive` will be set to `true`.

- `controlActiveState` is set to `.inactive`, `appearsActive` will be set to `false`.

## See Also

### Deprecated environment values

var disableAutocorrection: Bool?

A Boolean value that determines whether the view hierarchy has auto-correction enabled.

Deprecated

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

