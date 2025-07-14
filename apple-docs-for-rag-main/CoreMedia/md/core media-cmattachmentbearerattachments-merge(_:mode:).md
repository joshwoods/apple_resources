

- Core Media
- CMAttachmentBearerAttachments
-  merge(\_:mode:) 

Instance Method

# merge(\_:mode:)

Sets a collection of attachments on the object.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func merge(
    _ attachments: [String : Any],
    mode: CMAttachmentBearerAttachments.Mode
)
```

## Parameters 

`attachments`  

The attachments to set on this object.

`mode`  

The mode with which to add the attachments.

## See Also

### Managing Attachments

enum Mode

An enumeration that defines the available attachment modes.

func removeAll()

Removes all attachments from this object.

