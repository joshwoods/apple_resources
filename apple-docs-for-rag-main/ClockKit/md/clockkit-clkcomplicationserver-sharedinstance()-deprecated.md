

- ClockKit
- CLKComplicationServer
-  sharedInstance() Deprecated

Type Method

# sharedInstance()

Returns the shared complication server.

watchOS 2.0–9.0Deprecated

``` source
class func sharedInstance() -> Self
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

Always use this method to retrieve the shared complication server object. Don’t try to create instances of the object yourself.

