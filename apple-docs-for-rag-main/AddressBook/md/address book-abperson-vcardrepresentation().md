

- Address Book
- ABPerson
-  vCardRepresentation() 

Instance Method

# vCardRepresentation()

Returns the vCard representation of the person record as a data object in vCard format.

macOS

``` source
func vCardRepresentation() -> Data!
```

## Return Value

A data object containing the vCard representation of the person record.

## See Also

### Importing and Exporting vCard Formatted Files

init!(VCardRepresentation: Data!)

Returns an `ABPerson` instance initialized with the given data.

