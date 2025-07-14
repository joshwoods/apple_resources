

- Foundation
- NSExtensionContext
-  interfaceParametersDescription() 

Instance Method

# interfaceParametersDescription()

Returns a human-readable string describing the data that SiriKit displays to the user when you handle an intent.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func interfaceParametersDescription() -> String
```

## Discussion

If you provide an Intents UI app extension, you can customize all or some of the interface that SiriKit displays to the user for a given intent. The information displayed by SiriKit is different for each intent, and can change in the future. During development, use this method to retrieve a human-readable description of the contents of the doc://com.apple.documentation/documentation/sirikit/inparameter objects that SiriKit intends to display for the current intent. Use that information to plan your custom interface.

For information about customizing the Siri and Maps interfaces, see doc://com.apple.documentation/documentation/sirikit/creating_an_intents_ui_extension.

## See Also

### Getting Siri-related information

var hostedViewMinimumAllowedSize: CGSize

The minimum size for a Siri hosted view.

var hostedViewMaximumAllowedSize: CGSize

The maximum size for a Siri hosted view.

