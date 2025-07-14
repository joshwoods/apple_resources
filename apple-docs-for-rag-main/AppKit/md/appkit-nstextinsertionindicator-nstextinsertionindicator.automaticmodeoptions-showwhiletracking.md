

- AppKit
- NSTextInsertionIndicator
- NSTextInsertionIndicator.AutomaticModeOptions
-  showWhileTracking 

Type Property

# showWhileTracking

Specifies whether the insertion indicator shows during a tracking loop.

macOS 14.0+

``` source
static var showWhileTracking: NSTextInsertionIndicator.AutomaticModeOptions { get }
```

## Mentioned in 

Adopting the system text cursor in custom text views

## Discussion

When set, the insertion indicator hides during an NSEventTrackingRunLoopMode such as while actively scrolling a view.

## See Also

### Configuring automatic mode options

static var showEffectsView: NSTextInsertionIndicator.AutomaticModeOptions

Specifies whether a trailing glow displays during dictation.

