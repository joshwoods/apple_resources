

- ClockKit
- CLKComplicationTemplate
-  new() Deprecated

Type Method

# new()

Returns a new complication.

watchOS 2.0–7.0Deprecated

``` source
class func new() -> Self
```

Deprecated

Creating a template without parameters is deprecated in watchOS 7.0. Use a factory method with parameters instead.

## Discussion

You shouldn’t create instances of this class directly. Instead, you create instances of one of the concrete subclasses and use the resulting object to specify the data for your complication.

## See Also

### Creating Empty Templates

init()

Creates a new complication.

Deprecated

