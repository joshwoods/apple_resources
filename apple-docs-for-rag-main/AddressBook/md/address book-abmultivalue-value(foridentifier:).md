

- Address Book
- ABMultiValue
-  value(forIdentifier:) 

Instance Method

# value(forIdentifier:)

Returns the value for the given identifier.

macOS

``` source
func value(forIdentifier identifier: String!) -> Any!
```

## Parameters 

`identifier`  

The identifier for the value to be returned.

## Discussion

If the identifier is not found, returns `nil`.

## See Also

### Accessing entries

func label(at: Int) -> String!

Returns the label for the given index.

func value(at: Int) -> Any!

Returns the value for the given index.

func label(forIdentifier: String!) -> Any!

Returns the label for the given identifier.

