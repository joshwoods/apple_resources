

- Address Book
- ABMultiValue
-  label(forIdentifier:) 

Instance Method

# label(forIdentifier:)

Returns the label for the given identifier.

macOS

``` source
func label(forIdentifier identifier: String!) -> Any!
```

## Parameters 

`identifier`  

The identifier for the label to be returned.

## Discussion

If the identifier is not found, this method returns `nil`.

## See Also

### Accessing entries

func label(at: Int) -> String!

Returns the label for the given index.

func value(at: Int) -> Any!

Returns the value for the given index.

func value(forIdentifier: String!) -> Any!

Returns the value for the given identifier.

