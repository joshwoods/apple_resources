

- RealityKit
- Attachment
-  init(id:\_:) 

Initializer

# init(id:\_:)

Creates an new attachment from an identifier and a closure.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    id: AnyHashable,
    @ViewBuilder _ content: @escaping () -> Content
)
```

## Parameters 

`id`  

An `AnyHashable` instance that identifies the attachment and a ViewAttachmentEntity.

`content`  

A `ViewBuilder` instance that contains the views for the attachment.

## Discussion

You can access details of an attachment entity, such as its bounds, by calling the methods of a ViewAttachmentEntity instance. For example, you can add an attachment that contains the text `"hello"`.

```
Attachment(id: "example") {
    Text("hello")
}
```

Note

The initializer doesn’t automatically add the views to a RealityView instance. You need to explicitly add each entity to your app’s scene hierarchy by directly placing an entity attachment to the view or as a child of another entity that’s already in the view.

