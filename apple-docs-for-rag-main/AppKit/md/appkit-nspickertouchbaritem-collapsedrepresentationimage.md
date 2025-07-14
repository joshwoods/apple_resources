

- AppKit
- NSPickerTouchBarItem
-  collapsedRepresentationImage 

Instance Property

# collapsedRepresentationImage

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

**Mac Catalyst**

``` source
@MainActor
var collapsedRepresentationImage: UIImage? { get set }
```

**macOS**

``` source
@MainActor
var collapsedRepresentationImage: NSImage? { get set }
```

## See Also

### Configuring picker appearance

var numberOfOptions: Int

func setLabel(String, at: Int)

func label(at: Int) -> String?

func setImage(UIImage?, at: Int)

func image(at: Int) -> UIImage?

var collapsedRepresentationLabel: String

var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation

enum ControlRepresentation

Constants that specify display styles for picker bar items.

