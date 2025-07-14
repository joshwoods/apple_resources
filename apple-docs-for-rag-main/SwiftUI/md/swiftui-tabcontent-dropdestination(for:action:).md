

- SwiftUI
- TabContent
-  dropDestination(for:action:) 

Instance Method

# dropDestination(for:action:)

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func dropDestination(
    for payloadType: T.Type = T.self,
    action: @escaping ([T]) -> Void
) -> some TabContent where T : Transferable
```

## Parameters 

`payloadType`  

Type of the models that are dropped.

`action`  

A closure that takes the dropped content and responds appropriately. The closure takes one argument, which is an array of Transferable items that represents the data to insert.

## Return Value

A view that calls `action` when elements are dropped onto the tab.

## Discussion

The dropped content can be provided as binary data, file URLs, or file promises.

The drop destination is the tab content.

This example adds a profile to a group when the user drops it onto onto that group.

```
struct Profile: Identifiable {
    let givenName: String
    let familyName: String
    let image = "person.fill"
    let id = UUID().uuidString
}

@State private var profiles = [
    Profile(givenName: "Juan", familyName: "Chavez"),
    Profile(givenName: "Mei", familyName: "Chen"),
    Profile(givenName: "Tom", familyName: "Clark"),
    Profile(givenName: "Gita", familyName: "Kumar")
]

@State private var favoriteProfiles: [Profile] = []

var body: some View {
    TabView {
        Tab("All Profiles", systemImage: "list.bullet") {
            List(profiles) { profile in
                Text(profile.givenName)
                    .draggable(profile.id)
            }
        }

        Tab("Favorites", systemImage: "star.fill") {
            ForEach(favoritedProfiles) { profile in
                Tab(profile.givenName, image: profile.image) {
                    Label(profile.givenName, systemImage: "star.fill")
                }
            }
        }
        .dropDestination(for: String.self) { receivedIds in
             // Add profiles with `receivedIds` to favorites
        }
   }
```

