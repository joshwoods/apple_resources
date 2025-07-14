

- AppKit
- NSPickerTouchBarItem
-  image(at:) 

Instance Method

# image(at:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

**macOS**

``` source
@MainActor
func image(at index: Int) -> NSImage?
```

**Mac Catalyst**

``` source
@MainActor
func image(at index: Int) -> UIImage?
```

## See Also

### Configuring picker appearance

var numberOfOptions: Int

func setLabel(String, at: Int)

func label(at: Int) -> String?

func setImage(UIImage?, at: Int)

var collapsedRepresentationImage: UIImage?

var collapsedRepresentationLabel: String

var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation

enum ControlRepresentation

Constants that specify display styles for picker bar items.

