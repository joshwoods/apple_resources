

- FamilyControls
- FamilyActivityIconView
-  menuStyle(\_:) 

Instance Method

# menuStyle(\_:)

Sets the style for menus within this view.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+

``` source
nonisolated
func menuStyle(_ style: S) -> some View where S : MenuStyle
```

## Discussion

To set a specific style for all menu instances within a view, use the `menuStyle(_:)` modifier:

```
Menu("PDF") {
    Button("Open in Preview", action: openInPreview)
    Button("Save as PDF", action: saveAsPDF)
}
.menuStyle(ButtonMenuStyle())
```

