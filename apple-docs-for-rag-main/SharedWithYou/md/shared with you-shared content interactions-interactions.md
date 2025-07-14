

- Shared With You
-  Shared content interactions 

API Collection

# Shared content interactions

Use highlights and attribution views to manage participants and trigger events for shared content.

## Topics

### Attributions

class SWAttributionView

A view that displays the sender who shares a highlight and provides related actions.

### Highlights

class SWHighlight

An object that represents a universal link to share by any number of contacts in one or more conversations.

class SWHighlightCenter

An object that contains a priority-ordered list of universal links to share with the current user.

### Highlight events

protocol SWHighlightEvent

A protocol that defines an activity that the system posts in response to a user action for a highlight.

class SWHighlightChangeEvent

An object that represents change activity for a highlight.

class SWHighlightMembershipEvent

An object that represents membership activity for a highlight.

class SWHighlightMentionEvent

An object that represents mention activity for a highlight.

class SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

### Participants

class SWPerson

An object that tracks participants in a collaboration.

class SWRemoveParticipantAlert

An alert that prompts the user to remove a participant from a Messages group.

### Pasteboard Types

NSPasteboardTypeCollaborationMetadata

An object you use for conveying data during a collaboration.

## See Also

### Shared content

Making your app content shareable

Add support for universal links and a Shared with You shelf to support shared content in your app.

