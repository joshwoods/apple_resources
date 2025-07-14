

- Shared With You Core
- SWCollaborationShareOptions
-  init(optionsGroups:summary:) 

Initializer

# init(optionsGroups:summary:)

Creates and initializes a collaboration share options object the array of groups and a summary string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    optionsGroups: [SWCollaborationOptionsGroup],
    summary: String
)
```

## Parameters 

`optionsGroups`  

An array of SWCollaborationOptionsGroup objects to customize how the system shares the collaboration.

`summary`  

A localized string to summarize the collaboration options.

## See Also

### Creating share options

init(coder: NSCoder)

Creates and initializes a collaboration share options object.

convenience init(optionsGroups: [SWCollaborationOptionsGroup])

Creates and initializes a collaboration share options object with the array of groups.

