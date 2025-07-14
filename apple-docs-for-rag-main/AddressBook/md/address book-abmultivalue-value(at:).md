

- Address Book
- ABMultiValue
-  value(at:) 

Instance Method

# value(at:)

Returns the value for the given index.

macOS

``` source
func value(at index: Int) -> Any!
```

## Parameters 

`index`  

The index for the value to be returned.

## Discussion

If the `index` argument is out of bounds, this method raises an exception.

## See Also

### Accessing entries

func label(at: Int) -> String!

Returns the label for the given index.

func value(forIdentifier: String!) -> Any!

Returns the value for the given identifier.

func label(forIdentifier: String!) -> Any!

Returns the label for the given identifier.

