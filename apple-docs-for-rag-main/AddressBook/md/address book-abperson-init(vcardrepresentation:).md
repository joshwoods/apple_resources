

- Address Book
- ABPerson
-  init(VCardRepresentation:) 

Initializer

# init(VCardRepresentation:)

Returns an `ABPerson` instance initialized with the given data.

macOS

``` source
init!(VCardRepresentation vCardData: Data!)
```

``` source
init!(vCardRepresentation vCardData: Data!)
```

## Parameters 

`vCardData`  

A data object containing a vCard representation of a person record.

## Return Value

An `ABPerson` instance initialized with the given data.

## Discussion

Version 2.1 and 3.0 of the vCard format are supported. If `vCardData` is `nil` or is not a valid vCard format, this method returns `nil`.

## See Also

### Importing and Exporting vCard Formatted Files

func vCardRepresentation() -> Data!

Returns the vCard representation of the person record as a data object in vCard format.

