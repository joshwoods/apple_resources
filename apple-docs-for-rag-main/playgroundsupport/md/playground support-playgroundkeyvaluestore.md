

- Playground Support
-  PlaygroundKeyValueStore 

Class

# PlaygroundKeyValueStore

A data storage container you use to persist information across different sessions.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
class PlaygroundKeyValueStore
```

## Overview

The key-value store is available only in Swift Playgrounds and is persistent only in playground books.

The example below sets the value of the key “animal” in the playground key-value store to “Llama” and then retrieves the value of that key back from the key-value store.

// Store a value.
PlaygroundKeyValueStore.current.keyValueStore[&quot;animal&quot;] = .string(&quot;Llama&quot;)

// Retreive that same value.   
var theAnimal: String? = nil
if let keyValue = PlaygroundKeyValueStore.current.keyValueStore[&quot;animal&quot;],
    case .string(let animalType) = keyValue {
    theAnimal = animalType
}

## Topics

### Persisting Data

static let current: PlaygroundKeyValueStore

A reference to the key-value store for the current playground book.

subscript(String) -> PlaygroundValue?

Reads or stores the value associated with the given key in the key-value store.

## See Also

### Data Persistence

enum PlaygroundValue

The types you can save in the key-value store or send in messages to live views.

let playgroundSharedDataDirectory: URL

The path to the directory containing data shared between all playgrounds in Xcode.

