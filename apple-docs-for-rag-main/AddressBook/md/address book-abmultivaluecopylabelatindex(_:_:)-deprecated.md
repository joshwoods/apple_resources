

- Address Book
-  ABMultiValueCopyLabelAtIndex(\_:\_:) Deprecated

Function

# ABMultiValueCopyLabelAtIndex(\_:\_:)

Returns the label for the given index.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**iOS, iPadOS, Mac Catalyst**

``` source
func ABMultiValueCopyLabelAtIndex(
    _ multiValue: ABMultiValue!,
    _ index: CFIndex
) -> Unmanaged!
```

**macOS**

``` source
func ABMultiValueCopyLabelAtIndex(
    _ multiValue: ABMultiValueRef!,
    _ index: CFIndex
) -> Unmanaged!
```

Deprecated

use \[\[NSArray objectAtIndex:\] label\] with the labeled value property

## Parameters 

`multiValue`  

The multi-value list that you wish to access.

`index`  

The index of the identifier you wish to obtain. If this parameter is out of bounds, this function raises an exception.

## Return Value

The label at `index` in `multiValue`.You are responsible for releasing this object.

## Discussion

Each value in a multi-value list must be the same type, andhas an associated pre-defined or user-defined label, and uniqueidentifier. Use the ABMultiValueCopyIdentifierAtIndex(_:_:) functionto get a identifier, and the ABMultiValueCopyValueAtIndex(_:_:)functionto get a value.

## See Also

### Multi Values

func ABMultiValueAdd(ABMutableMultiValueRef!, CFTypeRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Bool

Adds a value and its label to a multi-value list.

func ABMultiValueCopyIdentifierAtIndex(ABMultiValueRef!, CFIndex) -> Unmanaged&lt;CFString>!

Returns the identifier at the given index.

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

