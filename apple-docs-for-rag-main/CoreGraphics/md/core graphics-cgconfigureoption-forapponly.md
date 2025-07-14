

- Core Graphics
- CGConfigureOption
-  forAppOnly 

Type Property

# forAppOnly

Changes persist for the lifetime of the current application. After the application terminates, the display configuration settings revert to the current login session.

Mac CatalystmacOS

``` source
static var forAppOnly: CGConfigureOption { get }
```

## See Also

### Type Properties

static var forSession: CGConfigureOption

Changes persist for the lifetime of the current login session. After the current session terminates, the displays revert to the last saved permanent configuration.

static var permanently: CGConfigureOption

