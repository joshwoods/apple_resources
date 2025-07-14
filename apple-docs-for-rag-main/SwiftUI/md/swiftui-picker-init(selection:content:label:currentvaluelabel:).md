

- SwiftUI
- Picker
-  init(selection:content:label:currentValueLabel:) 

Initializer

# init(selection:content:label:currentValueLabel:)

Creates a picker that displays a custom label and a custom value label where applicable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    selection: Binding,
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label,
    @ViewBuilder currentValueLabel: () -> some View
)
```

Available when `Label` conforms to `View`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

## Parameters 

`selection`  

A binding to a property that determines the currently-selected option.

`content`  

A view that contains the set of options.

`label`  

A view that describes the purpose of selecting an option.

`currentValueLabel`  

A view that represents the current value of the picker.

## Discussion

The following example shows a picker with a current value label that only displays the title of the currently selected song:

```
struct Song: Identifiable, Hashable {
    let id = UUID()
    let title: String
    let artist: String
    let genre: String
}

private let songs: [Song] = [ /* songs */]

@State private var selectedSong: Song? = nil

var body: some View {
    NavigationStack {
        List {
            Picker(selection: $selectedSong) {
                ForEach(songs) { song in
                    VStack(alignment: .leading) {
                        Text(song.title)
                            .bold()
                        Text(song.artist)
                        Text(song.genre)
                            .foregroundColor(.secondary)
                            .font(.caption)
                    }
                    .tag(song as Song?)
                }
            } label: {
                Text("Request a song")
            } currentValueLabel: {
                Text(selectedSong?.title ?? "No selection")
            }
        }
        .pickerStyle(.navigationLink)
    }
}
```

