

- SwiftUI
- WindowStyle
-  plain 

Type Property

# plain

The plain window style.

macOS 15.0+visionOS 1.0+

``` source
static var plain: PlainWindowStyle { get }
```

Available when `Self` is `PlainWindowStyle`.

## Discussion

Unlike automatic, a plain window does not receive a glass background in visionOS or window chrome in macOS. Use this style if you want more control over how these elements are used in your window.

## See Also

### Getting built-in window styles

static var automatic: DefaultWindowStyle

The default window style.

static var hiddenTitleBar: HiddenTitleBarWindowStyle

A window style which hides both the window’s title and the backing of the titlebar area, allowing more of the window’s content to show.

static var titleBar: TitleBarWindowStyle

A window style which displays the title bar section of the window.

static var volumetric: VolumetricWindowStyle

A window style that creates a 3D volumetric window.

