

- RealityKit
- RealityViewAttachments
-  entity(for:) 

Instance Method

# entity(for:)

Gets the identified attachment view as an entity, if the view with that identifier exists.

RealityKitSwiftUIvisionOS 1.0+

``` source
func entity(for id: some Hashable) -> ViewAttachmentEntity?
```

## Parameters 

`id`  

The value that you used to tag the view when you define it in the `attachments` parameter of the RealityView initializer init(make:update:attachments:).

## Return Value

The resolved attachment entity, or `nil` if RealityView can’t find an attachment view with the given `id`.

## Discussion

Attachment entities are not automatically added to your RealityView’s content. To display an attachment, add it to your RealityView’s content using a function like add(_:).

