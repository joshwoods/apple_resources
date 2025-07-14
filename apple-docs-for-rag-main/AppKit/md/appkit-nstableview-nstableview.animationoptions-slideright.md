

- AppKit
- NSTableView
- NSTableView.AnimationOptions
-  slideRight 

Type Property

# slideRight

Animates a row insertion by sliding from the right. Animates a row removal by sliding towards the right.

macOS 10.7+

``` source
static var slideRight: NSTableView.AnimationOptions { get }
```

## See Also

### Constants

static var effectFade: NSTableView.AnimationOptions

Use a fade for row or column removal. The effect can be combined with any of the slide constants.

static var effectGap: NSTableView.AnimationOptions

Creates a gap for newly inserted rows. This is useful for drag and drop animations that animate to a newly opened gap and should be used in the delegate method tableView(_:acceptDrop:row:dropOperation:).

static var slideUp: NSTableView.AnimationOptions

Animates a row insertion or removal by sliding upward.

static var slideDown: NSTableView.AnimationOptions

Animates a row insertion or removal by sliding downward.

static var slideLeft: NSTableView.AnimationOptions

Animates a row insertion by sliding from the left. Animates a row removal by sliding towards the left.

