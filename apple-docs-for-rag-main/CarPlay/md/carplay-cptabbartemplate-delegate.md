

- CarPlay
- CPTabBarTemplate
-  delegate 

Instance Property

# delegate

The object that acts as the template’s delegate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
weak var delegate: (any CPTabBarTemplateDelegate)? { get set }
```

## Discussion

The delegate must conform to the CPTabBarTemplateDelegate protocol.

## See Also

### Managing Tab Bar Interactions

protocol CPTabBarTemplateDelegate

The methods an object implements to act as the delegate for a tab bar template.

