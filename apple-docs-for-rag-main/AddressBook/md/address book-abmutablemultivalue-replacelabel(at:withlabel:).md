

- Address Book
- ABMutableMultiValue
-  replaceLabel(at:withLabel:) 

Instance Method

# replaceLabel(at:withLabel:)

Replaces the label at the given index.

macOS

``` source
func replaceLabel(
    at index: Int,
    withLabel label: String!
) -> Bool
```

## Parameters 

`index`  

The index of the label that will be replaced.

`label`  

The new label.

## Return Value

true if successful; otherwise, false.

## Discussion

If the label is `nil` or if the index is out of bounds, this method raises an exception.

## See Also

### Replacing values and labels

func replace(at: Int, withValue: Any!) -> Bool

Replaces the value at the given index.

