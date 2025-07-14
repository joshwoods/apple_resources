

- Address Book
- ABMutableMultiValue
-  replace(at:withValue:) 

Instance Method

# replace(at:withValue:)

Replaces the value at the given index.

macOS

``` source
func replace(
    at index: Int,
    withValue value: Any!
) -> Bool
```

## Parameters 

`index`  

The index of the value that will be replaced.

`value`  

The new value.

## Return Value

true if successful; otherwise false.

## Discussion

If the value is `nil` or if the index is out of bounds, this method raises an exception.

## See Also

### Replacing values and labels

func replaceLabel(at: Int, withLabel: String!) -> Bool

Replaces the label at the given index.

