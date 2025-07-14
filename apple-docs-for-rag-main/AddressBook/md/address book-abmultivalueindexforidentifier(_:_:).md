

- Address Book
-  ABMultiValueIndexForIdentifier(\_:\_:) 

Function

# ABMultiValueIndexForIdentifier(\_:\_:)

Returns the index for the given identifier.

macOS

``` source
func ABMultiValueIndexForIdentifier(
    _ multiValue: ABMultiValueRef!,
    _ identifier: CFString!
) -> CFIndex
```

## Parameters 

`multiValue`  

The multi-value list that you wish to access.

`identifier`  

The identifier whose index you wish to obtain.

## Return Value

The index of `identifier`.

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

func ABMultiValueInsert(ABMutableMultiValueRef!, CFTypeRef!, CFString!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Bool

Inserts a value and its label at the given index in amulti-value list.

func ABMultiValuePropertyType(ABMultiValueRef!) -> ABPropertyType

Returns the type for the values in a multi-value list.

func ABMultiValueRemove(ABMutableMultiValueRef!, CFIndex) -> Bool

Removes the value and label at the given index.

func ABMultiValueReplaceLabel(ABMutableMultiValueRef!, CFString!, CFIndex) -> Bool

Replaces the label at the given index.

func ABMultiValueReplaceValue(ABMutableMultiValueRef!, CFTypeRef!, CFIndex) -> Bool

Replaces the value at the given index.

