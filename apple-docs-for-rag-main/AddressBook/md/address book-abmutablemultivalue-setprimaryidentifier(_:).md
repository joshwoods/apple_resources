

- Address Book
- ABMutableMultiValue
-  setPrimaryIdentifier(\_:) 

Instance Method

# setPrimaryIdentifier(\_:)

Sets the primary value to be the value for the given identifier.

macOS

``` source
func setPrimaryIdentifier(_ identifier: String!) -> Bool
```

## Parameters 

`identifier`  

The identifier whose value will be used as the primary value for a multivalue property.

## Return Value

true if successful; otherwise false.

## Discussion

If the identifier is `nil`, this method raises an exception. Use the identifier(at:) method to get the identifier given the index.

