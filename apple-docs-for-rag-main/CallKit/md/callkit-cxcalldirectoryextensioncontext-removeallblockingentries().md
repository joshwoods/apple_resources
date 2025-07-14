

- CallKit
- CXCallDirectoryExtensionContext
-  removeAllBlockingEntries() 

Instance Method

# removeAllBlockingEntries()

Removes all stored blocking entries.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+visionOS 1.0+

``` source
func removeAllBlockingEntries()
```

## Discussion

If isIncremental is true, the request provides incremental entries and may use this method to remove all previously added blocking entries. Don’t call this method if isIncremental is false.

## See Also

### Removing Entries

func removeAllIdentificationEntries()

Removes all stored identification entries.

func removeBlockingEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes a blocking entry that contains the specified phone number.

func removeIdentificationEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes an identification entry that contains the specified phone number.

