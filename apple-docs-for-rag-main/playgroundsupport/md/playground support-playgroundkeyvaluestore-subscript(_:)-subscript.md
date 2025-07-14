

- Playground Support
- PlaygroundKeyValueStore
-  subscript(\_:) 

Subscript

# subscript(\_:)

Reads or stores the value associated with the given key in the key-value store.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
subscript(key: String) -> PlaygroundValue? { get set }
```

## Parameters 

`key`  

The key to find in the key-value store.

## Return Value

The value associated with the `key` parameter.

## See Also

### Persisting Data

static let current: PlaygroundKeyValueStore

A reference to the key-value store for the current playground book.

