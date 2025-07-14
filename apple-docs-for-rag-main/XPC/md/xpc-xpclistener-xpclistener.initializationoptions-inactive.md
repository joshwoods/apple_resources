

- XPC
- XPCListener
- XPCListener.InitializationOptions
-  inactive 

Type Property

# inactive

Indicates that the listener isn’t activated during its creation.

Mac Catalyst 17.0+macOS 14.0+

``` source
static var inactive: XPCListener.InitializationOptions
```

## Discussion

Important

If you create a listener with this option, you must manually activate it by calling activate().

## See Also

### Listener creation options

static var none: XPCListener.InitializationOptions

Indicates that the listener uses a default configuration during creation.

