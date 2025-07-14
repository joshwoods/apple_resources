

- Group Activities
- GroupSessionJournal
-  add(\_:metadata:) 

Instance Method

# add(\_:metadata:)

Adds the specified item and metadata to the journal and begins transferring the data to the other participants’ devices so they can access it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
final func add(
    _ item: ItemType,
    metadata: MetadataType
) async throws -> GroupSessionJournal.Attachment where ItemType : Transferable, MetadataType : Decodable, MetadataType : Encodable
```

## Parameters 

`item`  

The item to send to other session participants. The type you specify must conform to the Transferable protocol. For more information about creating transferable types, see Core Transferable.

`metadata`  

Custom metadata to include with the item. Specify a Codable type that contains information to help your app interpret or process the item on other devices. For example, you might include app-specific details that aren’t part of the item’s intrinsic data format.

## Return Value

An attachment object you can remove by passing it to the remove(attachment:) function.

## Discussion

Call this method when you want to send a file or codable data type to the other participants of an activity. The method runs asynchronously and can return before the upload operation finishes.

## See Also

### Uploading content to the session

func add&lt;ItemType>(ItemType) async throws -> GroupSessionJournal.Attachment

Adds the specified item to the journal and begins transferring the item’s data to the other participants’ devices so they can access it.

