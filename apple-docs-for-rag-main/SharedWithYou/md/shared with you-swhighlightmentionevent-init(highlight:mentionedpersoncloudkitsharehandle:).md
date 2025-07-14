

- Shared With You
- SWHighlightMentionEvent
-  init(highlight:mentionedPersonCloudKitShareHandle:) 

Initializer

# init(highlight:mentionedPersonCloudKitShareHandle:)

Creates and initializes a mention event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    highlight: SWHighlight,
    mentionedPersonCloudKitShareHandle handle: String
)
```

## Parameters 

`highlight`  

The related hightlight for the event.

`handle`  

The CloudKit handle of the person the sender mentions.

## See Also

### Creating a mention event

init(highlight: SWHighlight, mentionedPersonIdentity: SWPerson.Identity)

Creates and initializes a mention event.

