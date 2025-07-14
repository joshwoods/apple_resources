

- Shared With You
- SWHighlightMentionEvent
-  init(highlight:mentionedPersonIdentity:) 

Initializer

# init(highlight:mentionedPersonIdentity:)

Creates and initializes a mention event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    highlight: SWHighlight,
    mentionedPersonIdentity identity: SWPerson.Identity
)
```

## Parameters 

`highlight`  

The related hightlight for the event.

`identity`  

The `SWPersonIdentity` of the person the sender mentions.

## See Also

### Creating a mention event

init(highlight: SWHighlight, mentionedPersonCloudKitShareHandle: String)

Creates and initializes a mention event.

