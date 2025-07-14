

- CallKit
- CXCallDirectoryExtensionContext
-  removeBlockingEntry(withPhoneNumber:) 

Instance Method

# removeBlockingEntry(withPhoneNumber:)

Removes a blocking entry that contains the specified phone number.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+visionOS 1.0+

``` source
func removeBlockingEntry(withPhoneNumber phoneNumber: CXCallDirectoryPhoneNumber)
```

## Parameters 

`phoneNumber`  

The phone number to remove.

## Discussion

If isIncremental is true, the request provides incremental entries and may use this method to remove previously added blocking entries. This method removes all blocking entries that contain the specified phone number, even if multiple blocking entries with different labels are present for a single phone number.

Don’t call this method if isIncremental is false.

## See Also

### Removing Entries

func removeAllBlockingEntries()

Removes all stored blocking entries.

func removeAllIdentificationEntries()

Removes all stored identification entries.

func removeIdentificationEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes an identification entry that contains the specified phone number.

