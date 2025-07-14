

- Address Book
- ABMultiValue
-  index(forIdentifier:) 

Instance Method

# index(forIdentifier:)

Returns the index for the given identifier.

macOS

``` source
func index(forIdentifier identifier: String!) -> Int
```

## Parameters 

`identifier`  

The identifier whose index will be returned.

## Discussion

If the identifier is not found, returns `NSNotFound`.

## See Also

### Accessing identifiers

func identifier(at: Int) -> String!

Returns the identifier for the given index.

