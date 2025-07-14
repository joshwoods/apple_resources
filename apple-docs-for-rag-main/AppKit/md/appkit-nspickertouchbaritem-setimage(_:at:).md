

- AppKit
- NSPickerTouchBarItem
-  setImage(\_:at:) 

Instance Method

# setImage(\_:at:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

**macOS**

``` source
@MainActor
func setImage(
    _ image: NSImage?,
    at index: Int
)
```

**Mac Catalyst**

``` source
@MainActor
func setImage(
    _ image: UIImage?,
    at index: Int
)
```

## See Also

### Configuring picker appearance

var numberOfOptions: Int

func setLabel(String, at: Int)

func label(at: Int) -> String?

func image(at: Int) -> UIImage?

var collapsedRepresentationImage: UIImage?

var collapsedRepresentationLabel: String

var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation

enum ControlRepresentation

Constants that specify display styles for picker bar items.

