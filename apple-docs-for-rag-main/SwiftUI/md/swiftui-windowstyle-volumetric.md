

- SwiftUI
- WindowStyle
-  volumetric 

Type Property

# volumetric

A window style that creates a 3D volumetric window.

visionOS 1.0+

``` source
static var volumetric: VolumetricWindowStyle { get }
```

Available when `Self` is `VolumetricWindowStyle`.

## Discussion

Use a volumetric window — or a *volume* — to display 3D content within a bounded region. For example, Hello World uses a volume to present a `Globe` model that people can pick up and move around the Shared Space using the window bar:

```
WindowGroup(id: Module.globe.name) {
    Globe()
        .environment(model)
}
.windowStyle(.volumetric)
.defaultSize(width: 0.6, height: 0.6, depth: 0.6, in: .meters)
```

A volume enables someone to view content from all angles, unlike other windows which fade out as people move around the window. Also unlike other windows, a volume uses fixed scale, which means that objects in the volume appear smaller when the volume is farther away, like real objects would. For a comparison of fixed and dynamic scale, see Spatial layout in the Human Interface Guidelines.

You can specify a size for the volume using one of the default size scene modifiers, like defaultSize(width:height:depth:in:). Because volumes use fixed scale, it’s typically convenient to specify a size in physical units — like meters, as the above code demonstrates. People can’t change the size of the volume after it appears.

For design guidance, see Windows in the Human Interface Guidelines. If you want to place 3D objects arbitrarily throughout the Shared Space or in a Full Space, use an ImmersiveSpace instead.

## See Also

### Getting built-in window styles

static var automatic: DefaultWindowStyle

The default window style.

static var hiddenTitleBar: HiddenTitleBarWindowStyle

A window style which hides both the window’s title and the backing of the titlebar area, allowing more of the window’s content to show.

static var plain: PlainWindowStyle

The plain window style.

static var titleBar: TitleBarWindowStyle

A window style which displays the title bar section of the window.

