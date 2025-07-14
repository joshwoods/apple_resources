

- Foundation
- NSExtensionContext
-  hostedViewMaximumAllowedSize 

Instance Property

# hostedViewMaximumAllowedSize

The maximum size for a Siri hosted view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var hostedViewMaximumAllowedSize: CGSize { get }
```

## Discussion

Apps can customize the Siri interface using an Intents UI extension. The extension vends a view controller whose view contains the custom content that you want Siri to display. The size of that view controller’s view must be no larger than the size value in this property.

## See Also

### Getting Siri-related information

var hostedViewMinimumAllowedSize: CGSize

The minimum size for a Siri hosted view.

func interfaceParametersDescription() -> String

Returns a human-readable string describing the data that SiriKit displays to the user when you handle an intent.

