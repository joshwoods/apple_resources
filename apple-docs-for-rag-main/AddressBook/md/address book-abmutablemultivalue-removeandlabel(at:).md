

- Address Book
- ABMutableMultiValue
-  removeAndLabel(at:) 

Instance Method

# removeAndLabel(at:)

Removes the value and label at the given index.

macOS

``` source
func removeAndLabel(at index: Int) -> Bool
```

## Parameters 

`index`  

The index of the value-label pair that will be removed.

## Return Value

true if successful; otherwise false.

## Discussion

If the index is out of bounds, this method raises an exception.

