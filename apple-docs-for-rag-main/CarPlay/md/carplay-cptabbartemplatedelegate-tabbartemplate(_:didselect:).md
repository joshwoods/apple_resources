

- CarPlay
- CPTabBarTemplateDelegate
-  tabBarTemplate(\_:didSelect:) 

Instance Method

# tabBarTemplate(\_:didSelect:)

Tells the delegate when the tab bar selects the specified template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func tabBarTemplate(
    _ tabBarTemplate: CPTabBarTemplate,
    didSelect selectedTemplate: CPTemplate
)
```

**Required**

## Parameters 

`tabBarTemplate`  

The tab bar template that alerts you to the change in selection.

`selectedTemplate`  

The template that the user selects.

## Discussion

The tab bar template calls this method each time the user selects a tab. `tabBarTemplate` is the same template that the tab bar’s selectedTemplate property returns.

