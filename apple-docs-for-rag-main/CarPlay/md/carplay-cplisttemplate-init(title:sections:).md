

- CarPlay
- CPListTemplate
-  init(title:sections:) 

Initializer

# init(title:sections:)

Creates a list template with an array of list sections and optional title.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    title: String?,
    sections: [CPListSection]
)
```

## Parameters 

`title`  

A title that appears in the navigation bar while the template is visible.

`sections`  

An array of list sections, each with zero or more list items.

## Return Value

A newly initialized list template.

## See Also

### Creating a List Template

init(title: String?, sections: [CPListSection], assistantCellConfiguration: CPAssistantCellConfiguration?)

Creates a sectioned list template that optionally displays the assistant cell.

