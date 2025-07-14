

- SwiftUI
- DynamicViewContent
-  dropDestination(for:action:) 

Instance Method

# dropDestination(for:action:)

Sets the insert action for the dynamic view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func dropDestination(
    for payloadType: T.Type = T.self,
    action: @escaping ([T], Int) -> Void
) -> some DynamicViewContent where T : Transferable
```

## Parameters 

`payloadType`  

Type of the models that are dropped.

`action`  

A closure that SwiftUI invokes when elements are added to the view. The closure takes two arguments: The first argument is the offset relative to the dynamic view’s underlying collection of data. The second argument is an array of `Transferable` items that represents the data that you want to insert.

## Return Value

A view that calls `action` when elements are inserted into the original view.

## Discussion

```
struct Profile: Identifiable {
    let givenName: String
    let familyName: String
    let id = UUID()
}

@State private var profiles: [Profile] = [
    Person(givenName: "Juan", familyName: "Chavez"),
    Person(givenName: "Mei", familyName: "Chen"),
    Person(givenName: "Tom", familyName: "Clark"),
    Person(givenName: "Gita", familyName: "Kumar")
]

var body: some View {
    List {
        ForEach(profiles) { profile in
            Text(profile.givenName)
        }
        .dropDestination(for: Profile.self) { receivedProfiles, offset in
            profiles.insert(contentsOf: receivedProfiles, at: offset)
        }
    }
}
```

## See Also

### Responding to updates

func onDelete(perform: Optional&lt;(IndexSet) -> Void>) -> some DynamicViewContent

Sets the deletion action for the dynamic view. You must delete the corresponding item within `action`, as it will be called after the row has already been removed from the List.

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

func onMove(perform: Optional&lt;(IndexSet, Int) -> Void>) -> some DynamicViewContent

Sets the move action for the dynamic view.

