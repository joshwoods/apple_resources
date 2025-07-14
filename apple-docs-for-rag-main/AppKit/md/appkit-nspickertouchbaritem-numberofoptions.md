

- AppKit
- NSPickerTouchBarItem
-  numberOfOptions 

Instance Property

# numberOfOptions

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
var numberOfOptions: Int { get set }
```

## See Also

### Configuring picker appearance

func setLabel(String, at: Int)

func label(at: Int) -> String?

func setImage(UIImage?, at: Int)

func image(at: Int) -> UIImage?

var collapsedRepresentationImage: UIImage?

var collapsedRepresentationLabel: String

var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation

enum ControlRepresentation

Constants that specify display styles for picker bar items.

