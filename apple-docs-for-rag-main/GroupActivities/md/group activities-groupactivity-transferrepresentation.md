

- Group Activities
- GroupActivity
-  transferRepresentation 

Type Property

# transferRepresentation

A default type that lets the system share your activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static var transferRepresentation: some TransferRepresentation { get }
```

Available when `Self` conforms to `Transferable`.

## Discussion

This property contains a default GroupActivityTransferRepresentation for your activity. The system uses this type to offer your activity via SharePlay.

