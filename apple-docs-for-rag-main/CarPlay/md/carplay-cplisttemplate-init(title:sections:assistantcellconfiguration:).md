

- CarPlay
- CPListTemplate
-  init(title:sections:assistantCellConfiguration:) 

Initializer

# init(title:sections:assistantCellConfiguration:)

Creates a sectioned list template that optionally displays the assistant cell.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(
    title: String?,
    sections: [CPListSection],
    assistantCellConfiguration: CPAssistantCellConfiguration?
)
```

## Parameters 

`title`  

The title that the navigation bar displays while the template is visible.

`sections`  

An array of sections, each with zero or more list items. For more information, see CPListSection.

`assistantCellConfiguration`  

The object that provides the configuration attributes for the assistant cell, such as position and visibility. For more information, see CPAssistantCellConfiguration.

## Discussion

The system provides the text and accessory image for the assistant cell and you can’t change these. Use the assistantCellConfiguration property to update the cell’s configuration after you initialize the template. CarPlay observes this property and automatically updates your app’s interface in response to any changes.

Your app doesn’t receive a callback when the user selects the assistant cell. Instead, you configure an Intents Extension to handle the type of intent you specify in the cell’s configuration; audio apps must support doc://com.apple.documentation/documentation/sirikit/inplaymediaintent and communication apps must support doc://com.apple.documentation/documentation/sirikit/instartcallintent.

## See Also

### Creating a List Template

init(title: String?, sections: [CPListSection])

Creates a list template with an array of list sections and optional title.

