

- Group Activities
- GroupSessionJournal
-  attachments 

Instance Property

# attachments

The currently available attachments for you to download and incorporate into your app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
final var attachments: GroupSessionJournal.Attachments { get set }
```

## Discussion

This property contains an asynchronous sequence that you monitor while the current session is active. To monitor this sequence, configure an asynchronous task and iterate over the contents of the GroupSessionJournal.Attachments type. For an example of how to configure this task, see the overview for GroupSessionJournal.

The system updates this array whenever a participant adds or removes an attachment. Iterate over the array and update your app’s data structures to match the current contents.

## See Also

### Downloading content from the session

struct Attachments

An asynchronous sequence that contains one or more incoming attachment containers for you to process.

struct Attachment

A container for the data you download.

