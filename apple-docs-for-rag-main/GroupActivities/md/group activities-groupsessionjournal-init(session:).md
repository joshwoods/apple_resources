

- Group Activities
- GroupSessionJournal
-  init(session:) 

Initializer

# init(session:)

Creates a journal and associates it with the specified session of a group activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(session: GroupSession) where Activity : GroupActivity
```

## Parameters 

`session`  

The session you use for communicating with participants. The session must be in the GroupSession.State.waiting or GroupSession.State.joined state when you create the journal, and the session must be in the GroupSession.State.joined state before you can send or receive attachments.

## Return Value

A GroupSessionJournal object configured for the specified session.

