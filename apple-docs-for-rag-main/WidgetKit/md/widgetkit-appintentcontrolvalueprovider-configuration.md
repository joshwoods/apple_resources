

- WidgetKit
- AppIntentControlValueProvider
-  Configuration 

Associated Type

# Configuration

The type of intent used to prepare the value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
associatedtype Configuration : ControlConfigurationIntent
```

**Required**

## Discussion

When you create a custom provider, Swift infers this type from your implementation of the required `ValueProvider/previewValue(configuration:)` and `ValueProvider/currentValue(configuration:)` methods.

