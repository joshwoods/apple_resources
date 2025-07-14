

- Address Book
- ABMultiValue
-  identifier(at:) 

Instance Method

# identifier(at:)

Returns the identifier for the given index.

macOS

``` source
func identifier(at index: Int) -> String!
```

## Parameters 

`index`  

The index of the identifier to be returned.

## Discussion

If the `index` argument is out of bounds, this method raises an exception.

## See Also

### Accessing identifiers

func index(forIdentifier: String!) -> Int

Returns the index for the given identifier.

