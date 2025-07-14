

- CarPlay
-  CPTabBarTemplateDelegate 

Protocol

# CPTabBarTemplateDelegate

The methods an object implements to act as the delegate for a tab bar template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol CPTabBarTemplateDelegate : NSObjectProtocol
```

## Overview

You use the `CPTabBarTemplateDelegate` protocol to respond to a tab bar template’s events. The protocol defines methods that the template calls in response to these events, and your implementation provides the appropriate behavior when the events occur. For example, reloading a tab’s contents when the user selects it to make sure it’s displaying the latest data.

## Topics

### Managing the Selected Template

func tabBarTemplate(CPTabBarTemplate, didSelect: CPTemplate)

Tells the delegate when the tab bar selects the specified template.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Tab Bar Interactions

var delegate: (any CPTabBarTemplateDelegate)?

The object that acts as the template’s delegate.

