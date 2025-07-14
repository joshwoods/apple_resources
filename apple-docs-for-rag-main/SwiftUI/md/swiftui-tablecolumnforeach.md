

- SwiftUI
-  TableColumnForEach 

Structure

# TableColumnForEach

A structure that computes columns on demand from an underlying collection of identified data.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
struct TableColumnForEach where Data : RandomAccessCollection, ID : Hashable, RowValue == Content.TableRowValue, Sort == Content.TableColumnSortComparator, Content : TableColumnContent
```

## Overview

Use `TableColumnForEach` to create columns based on a RandomAccessCollection of some data type. Either the collection’s elements must conform to Identifiable or you need to provide an `id` parameter to the `TableColumnForEach` initializer.

The following example shows the interface for an `AudioSampleTrack`, which h as a collection of `AudioSample` across a dynamic number of `AudioChannel`s. The `Table` is created for displaying rows for each sample. It has one static column for the sample’s timestamp and uses a `TableColumnForEach` instance to produce a column for each of the audio channels in the track.

```
struct AudioChannel: Identifiable {
    let name: String
    let id: UUID
}

struct AudioSample: Identifiable {
    let id: UUID
    let timestamp: TimeInterval
    func level(channel: AudioChannel.ID) -> Double
}

@Observable
class AudioSampleTrack {
    let channels: [AudioChannel]
    var samples: some RandomAccessCollection { get }
}

struct ContentView: View {
    var track: AudioSampleTrack

    var body: some View {
        Table(track.samples) {
            TableColumn("Timestamp (ms)") { sample in
                Text(sample.timestamp, format: .number.scale(1000))
                    .monospacedDigit()
            }
            TableColumnForEach(track.channels) { channel in
                TableColumn(channel.name) { sample in
                    Text(sample.level(channel: channel.id),
                         format: .number.precision(.fractionLength(2))
                    )
                    .monospacedDigit()
                }
                .width(ideal: 70)
                .alignment(.numeric)
            }
        }
    }
}
```

## Topics

### Creating the collection

init(_:content:)

Creates an instance that uniquely identifies and creates table columns across updates based on the identity of the underlying data.

init(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> Content)

Creates an instance that uniquely identifies and creates table columns across updates based on the provided key path to the underlying data’s identifier.

### Accessing collection content

var content: (Data.Element) -> Content

A function to create content on demand using the underlying data.

var data: Data

The collection of underlying identified data that SwiftUI uses to create columns dynamically.

## Relationships

### Conforms To

- TableColumnContent

## See Also

### Creating columns

struct TableColumn

A column that displays a view for each row in a table.

protocol TableColumnContent

A type used to represent columns within a table.

struct TableColumnAlignment

Describes the alignment of the content of a table column.

struct TableColumnBuilder

A result builder that creates table column content from closures.

