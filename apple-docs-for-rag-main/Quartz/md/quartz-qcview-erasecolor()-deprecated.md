

- Quartz
- QCView
-  eraseColor() Deprecated

Instance Method

# eraseColor()

Retrieves the current color used to erase the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func eraseColor() -> NSColor!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The color object previously set using the setEraseColor(_:) method.

## See Also

### Managing the Erase Color

func erase()

Clears the view using the current erase color.

Deprecated

func setEraseColor(NSColor!)

Sets the color used to erase the view.

Deprecated

