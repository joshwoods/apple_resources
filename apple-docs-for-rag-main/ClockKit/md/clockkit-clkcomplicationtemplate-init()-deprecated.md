

- ClockKit
- CLKComplicationTemplate
-  init() Deprecated

Initializer

# init()

Creates a new complication.

watchOS 2.0–7.0Deprecated

``` source
init()
```

Deprecated

Initializing a template without parameters is deprecated in watchOS 7.0. Use an init with parameters instead.

## Discussion

You shouldn’t create instances of this class directly. Instead, you create instances of one of the concrete subclasses and use the resulting object to specify the data for your complication.

## See Also

### Creating Empty Templates

class func new() -> Self

Returns a new complication.

Deprecated

