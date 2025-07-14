

- SwiftUI
-  VolumetricWindowStyle 

Structure

# VolumetricWindowStyle

A window style that creates a 3D volumetric window.

visionOS 1.0+

``` source
struct VolumetricWindowStyle
```

## Overview

Use volumetric to construct this style:

```
WindowGroup {
    ContentView()
}
.windowStyle(.volumetric)
```

## Topics

### Creating the window style

init()

## Relationships

### Conforms To

- WindowStyle

## See Also

### Supporting types

struct DefaultWindowStyle

The default window style.

struct HiddenTitleBarWindowStyle

A window style which hides both the window’s title and the backing of the titlebar area, allowing more of the window’s content to show.

struct PlainWindowStyle

The plain window style.

struct TitleBarWindowStyle

A window style which displays the title bar section of the window.

