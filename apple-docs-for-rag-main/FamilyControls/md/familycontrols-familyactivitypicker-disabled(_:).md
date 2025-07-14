

- FamilyControls
- FamilyActivityPicker
-  disabled(\_:) 

Instance Method

# disabled(\_:)

Adds a condition that controls whether users can interact with this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func disabled(_ disabled: Bool) -> some View
```

## Parameters 

`disabled`  

A Boolean value that determines whether users can interact with this view.

## Return Value

A view that controls whether users can interact with this view.

## Discussion

The higher views in a view hierarchy can override the value you set on this view. In the following example, the button isn’t interactive because the outer `disabled(_:)` modifier overrides the inner one:

```
HStack {
    Button(Text("Press")) {}
    .disabled(false)
}
.disabled(true)
```

## See Also

### Interactivity

func handlesExternalEvents(preferring: Set&lt;String>, allowing: Set&lt;String>) -> some View

Specifies the external events that the view’s scene handles if the scene is already open.

