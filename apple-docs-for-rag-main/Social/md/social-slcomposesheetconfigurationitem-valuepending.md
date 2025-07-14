

- Social
- SLComposeSheetConfigurationItem
-  valuePending 

Instance Property

# valuePending

A Boolean value that indicates whether the configuration item’s value is ready for display.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
var valuePending: Bool { get set }
```

## Discussion

Set this property to true if a progress indicator should be displayed, to show users that a configuration item’s value is about to display. The default value of this property is false.

## See Also

### Specifying Configuration Information

var title: String!

The name of the configuration item stored as a localized string.

var value: String!

The current value or setting of the configuration item.

