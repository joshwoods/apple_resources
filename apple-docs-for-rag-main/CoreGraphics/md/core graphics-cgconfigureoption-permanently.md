

- Core Graphics
- CGConfigureOption
-  permanently 

Type Property

# permanently

Mac CatalystmacOS

``` source
static var permanently: CGConfigureOption { get }
```

## Discussion

Changes persist in future login sessions by the same user. If the requested changes cannot be supported by the Aqua UI (resolution and pixel depth constraints apply), the settings for the current login session are used instead, and any changes have session scope.

## See Also

### Type Properties

static var forAppOnly: CGConfigureOption

Changes persist for the lifetime of the current application. After the application terminates, the display configuration settings revert to the current login session.

static var forSession: CGConfigureOption

Changes persist for the lifetime of the current login session. After the current session terminates, the displays revert to the last saved permanent configuration.

