

- AppKit
- NSColorWell
- NSColorWell.Style
-  NSColorWell.Style.expanded 

Case

# NSColorWell.Style.expanded

A style that supports a color picker popover for fast interactions, and adds a dedicated button to display the color panel.

macOS 13.0+

``` source
case expanded
```

## Discussion

This style displays a dedicated button and a rectangular area with the selected color. Clicks in the dedicated button always display the system color panel. Clicks in the color area display a popover with a color picker. If you specified a custom action using the pulldownAction and pulldownTarget properties, clicks in the color area execute your action method instead.

## See Also

### Getting the Style Option

case `default`

The default style for color wells.

case minimal

A style that adds minimal adornments to the color well.

