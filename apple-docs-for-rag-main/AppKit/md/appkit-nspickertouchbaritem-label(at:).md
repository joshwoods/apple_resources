

- AppKit
- NSPickerTouchBarItem
-  label(at:) 

Instance Method

# label(at:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
func label(at index: Int) -> String?
```

## See Also

### Configuring picker appearance

var numberOfOptions: Int

func setLabel(String, at: Int)

func setImage(UIImage?, at: Int)

func image(at: Int) -> UIImage?

var collapsedRepresentationImage: UIImage?

var collapsedRepresentationLabel: String

var controlRepresentation: NSPickerTouchBarItem.ControlRepresentation

enum ControlRepresentation

Constants that specify display styles for picker bar items.

