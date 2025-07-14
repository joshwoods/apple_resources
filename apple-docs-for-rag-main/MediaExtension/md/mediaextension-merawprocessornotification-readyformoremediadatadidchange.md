

- MediaExtension
- MERAWProcessorNotification
-  readyForMoreMediaDataDidChange 

Type Property

# readyForMoreMediaDataDidChange

A notification that indicates a change to the object’s readiness to process additional media data.

macOS 15.0+

``` source
static let readyForMoreMediaDataDidChange: NSNotification.Name
```

## Discussion

This notification is used to notify Video Toolbox that the value of the isReadyForMoreMediaData property has changed.

