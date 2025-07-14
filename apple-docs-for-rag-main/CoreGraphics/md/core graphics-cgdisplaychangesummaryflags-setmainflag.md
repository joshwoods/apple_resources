

- Core Graphics
- CGDisplayChangeSummaryFlags
-  setMainFlag 

Type Property

# setMainFlag

The display is now the main display.

Mac CatalystmacOS

``` source
static var setMainFlag: CGDisplayChangeSummaryFlags { get }
```

## See Also

### Constants

static var beginConfigurationFlag: CGDisplayChangeSummaryFlags

The display configuration is about to change.

static var movedFlag: CGDisplayChangeSummaryFlags

The location of the upper-left corner of the display in the global display coordinate space has changed.

static var setModeFlag: CGDisplayChangeSummaryFlags

The display mode has changed.

static var addFlag: CGDisplayChangeSummaryFlags

The display has been added to the active display list.

static var removeFlag: CGDisplayChangeSummaryFlags

The display has been removed from the active display list.

static var enabledFlag: CGDisplayChangeSummaryFlags

The display has been enabled.

static var disabledFlag: CGDisplayChangeSummaryFlags

The display has been disabled.

static var mirrorFlag: CGDisplayChangeSummaryFlags

The display is now mirroring another display.

static var unMirrorFlag: CGDisplayChangeSummaryFlags

The display is no longer mirroring another display.

static var desktopShapeChangedFlag: CGDisplayChangeSummaryFlags

