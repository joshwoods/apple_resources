

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  importableFromServices(for:action:) 

Instance Method

# importableFromServices(for:action:)

Enables importing items from services, such as Continuity Camera on macOS.

RealityKitSwiftUImacOS 13.0+

``` source
nonisolated
func importableFromServices(
    for payloadType: T.Type = T.self,
    action: @escaping ([T]) -> Bool
) -> some View where T : Transferable
```

## Parameters 

`payloadType`  

The expected type of the imported models.

`action`  

A closure that will be called with the imported service item. Return `false` to indicate that there was a failure to receive the items.

## Discussion

```
@State private var title: String
var body: some View {
    Color.pink
        .frame(width: 400, height: 400)
        .importableFromServices(for: String.self) { titles
            title = titles.first ?? title
            return !titles.isEmpty
        }
}
```

