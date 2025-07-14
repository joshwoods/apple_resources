

- Address Book
- ABMultiValue
-  propertyType() 

Instance Method

# propertyType()

Returns the type for the values in a multivalue list.

macOS

``` source
func propertyType() -> ABPropertyType
```

## Discussion

If the multivalue list is empty or its values are of different types, it returns `kABErrorInProperty`.

## See Also

### Querying the list

func count() -> Int

Returns the number of entries in a multivalue list.

