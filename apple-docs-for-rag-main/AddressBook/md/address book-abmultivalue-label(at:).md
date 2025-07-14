

- Address Book
- ABMultiValue
-  label(at:) 

Instance Method

# label(at:)

Returns the label for the given index.

macOS

``` source
func label(at index: Int) -> String!
```

## Parameters 

`index`  

The index for the label to be returned.

## Discussion

If the `index` argument is out of bounds, this method raises an exception.

## See Also

### Accessing entries

func value(at: Int) -> Any!

Returns the value for the given index.

func value(forIdentifier: String!) -> Any!

Returns the value for the given identifier.

func label(forIdentifier: String!) -> Any!

Returns the label for the given identifier.

