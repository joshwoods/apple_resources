

- WidgetKit
- ControlValueProvider
-  Value 

Associated Type

# Value

The type of value provided to the template.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
associatedtype Value
```

**Required**

## Discussion

When you create a custom provider, Swift infers this type from your implementation of the required previewValue property and currentValue() method.

