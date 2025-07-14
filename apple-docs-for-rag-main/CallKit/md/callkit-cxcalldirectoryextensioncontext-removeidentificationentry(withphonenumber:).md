

- CallKit
- CXCallDirectoryExtensionContext
-  removeIdentificationEntry(withPhoneNumber:) 

Instance Method

# removeIdentificationEntry(withPhoneNumber:)

Removes an identification entry that contains the specified phone number.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+visionOS 1.0+

``` source
func removeIdentificationEntry(withPhoneNumber phoneNumber: CXCallDirectoryPhoneNumber)
```

## Parameters 

`phoneNumber`  

The phone number to remove.

## Discussion

If isIncremental is true, the request provides incremental entries and may use this method to remove previously added identification entries. This method removes all identification entries that contain the specified phone number, even if multiple identification entries with different labels are present for a single phone number.

Don’t call this method if isIncremental is false.

## See Also

### Removing Entries

func removeAllBlockingEntries()

Removes all stored blocking entries.

func removeAllIdentificationEntries()

Removes all stored identification entries.

func removeBlockingEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes a blocking entry that contains the specified phone number.

