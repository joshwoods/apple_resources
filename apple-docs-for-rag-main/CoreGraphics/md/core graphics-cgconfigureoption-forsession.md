

- Core Graphics
- CGConfigureOption
-  forSession 

Type Property

# forSession

Changes persist for the lifetime of the current login session. After the current session terminates, the displays revert to the last saved permanent configuration.

Mac CatalystmacOS

``` source
static var forSession: CGConfigureOption { get }
```

## See Also

### Type Properties

static var forAppOnly: CGConfigureOption

Changes persist for the lifetime of the current application. After the application terminates, the display configuration settings revert to the current login session.

static var permanently: CGConfigureOption

