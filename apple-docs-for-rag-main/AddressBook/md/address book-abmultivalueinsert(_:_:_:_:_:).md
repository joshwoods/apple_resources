

- Address Book
-  ABMultiValueInsert(\_:\_:\_:\_:\_:) 

Function

# ABMultiValueInsert(\_:\_:\_:\_:\_:)

Inserts a value and its label at the given index in amulti-value list.

macOS

``` source
func ABMultiValueInsert(
    _ multiValue: ABMutableMultiValueRef!,
    _ value: CFTypeRef!,
    _ label: CFString!,
    _ index: CFIndex,
    _ outIdentifier: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`multiValue`  

The multi-value list you wish to modify.

`value`  

An object representing a value in a multi-value list–it must be of the correct type. For example, if `multiValue` is the value for a property of type kABMultiStringProperty, then `value` needs to be a CFString object. See Property Types for a list of supported types in a multi-value list(see descriptions of the `kABMulti...` constants). If `value` is `NULL`, this function raises an exception.

`label`  

The label for `value`—it need not be unique. If `label` is `NULL`, this function raises an exception.

`index`  

The index to insert `value` at. If `index` is out of bounds, this function raises an exception.

`outIdentifier`  

If `value` is added successfully, this parameter returns the new identifier.

## Return Value

`true` ifsuccessfully, `false` otherwise.

## Discussion

This function performs no type checking and will let you adda value whose type does not match the types of the other valuesin the list. However, if you try to use a multi-value list whosevalues are not all of the same type, functions, such as the ABRecord ABRecordSetValue(_:_:_:_:) function,will returns `NULL` or kABErrorProperty.

## See Also

### Multi Values

func ABMultiValueAdd(ABMutableMultiValueRef!, CFTypeRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Bool

Adds a value and its label to a multi-value list.

func ABMultiValueCopyIdentifierAtIndex(ABMultiValueRef!, CFIndex) -> Unmanaged&lt;CFString>!

Returns the identifier at the given index.

func ABMultiValueCopyLabelAtIndex(ABMultiValue!, CFIndex) -> Unmanaged&lt;CFString>!

Returns the label for the given index.

Deprecated

func ABMultiValueCopyPrimaryIdentifier(ABMultiValueRef!) -> Unmanaged&lt;CFString>!

Returns the identifier for the primary value.

func ABMultiValueCopyValueAtIndex(ABMultiValue!, CFIndex) -> Unmanaged&lt;CFTypeRef>!

Returns the value for the given index.

Deprecated

func ABMultiValueCount(ABMultiValueRef!) -> CFIndex

Returns the number of entries in a multi-value list.

func ABMultiValueCreate() -> Unmanaged&lt;ABMultiValueRef>!

Returns a new ABMultiValue object.

func ABMultiValueCreateCopy(ABMultiValueRef!) -> Unmanaged&lt;ABMultiValueRef>!

Returns a copy of a multi-value object.

func ABMultiValueCreateMutable(ABPropertyType) -> Unmanaged&lt;ABMutableMultiValue>!

Returns a newly created mutable multi-value list object.

Deprecated

func ABMultiValueCreateMutableCopy(ABMultiValue!) -> Unmanaged&lt;ABMutableMultiValue>!

Returns a mutable copy of a multi-value object.

Deprecated

func ABMultiValueIndexForIdentifier(ABMultiValueRef!, CFString!) -> CFIndex

Returns the index for the given identifier.

func ABMultiValuePropertyType(ABMultiValueRef!) -> ABPropertyType

Returns the type for the values in a multi-value list.

func ABMultiValueRemove(ABMutableMultiValueRef!, CFIndex) -> Bool

Removes the value and label at the given index.

func ABMultiValueReplaceLabel(ABMutableMultiValueRef!, CFString!, CFIndex) -> Bool

Replaces the label at the given index.

func ABMultiValueReplaceValue(ABMutableMultiValueRef!, CFTypeRef!, CFIndex) -> Bool

Replaces the value at the given index.

