

- AppKit
- NSPickerTouchBarItem
-  controlRepresentation 

Instance Property

# controlRepresentation

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation { get set }
```

## See Also

### Configuring picker appearance

var numberOfOptions: Int

func setLabel(String, at: Int)

func label(at: Int) -> String?

func setImage(UIImage?, at: Int)

func image(at: Int) -> UIImage?

var collapsedRepresentationImage: UIImage?

var collapsedRepresentationLabel: String

enum ControlRepresentation

Constants that specify display styles for picker bar items.

