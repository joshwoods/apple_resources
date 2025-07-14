

- CallKit
- CXCallDirectoryExtensionContext
-  addBlockingEntry(withNextSequentialPhoneNumber:) 

Instance Method

# addBlockingEntry(withNextSequentialPhoneNumber:)

Adds a blocking entry with the specified phone number.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func addBlockingEntry(withNextSequentialPhoneNumber phoneNumber: CXCallDirectoryPhoneNumber)
```

## Parameters 

`phoneNumber`  

The phone number to be blocked.

## Mentioned in 

Identifying and blocking calls

## Discussion

When a phone number is blocked, the system telephony provider will disallow incoming calls from that phone number without displaying them to the user.

Call this method on the instance of CXCallDirectoryExtensionContext passed as an argument to the block parameter of the CXCallDirectoryProvider instance method beginRequest(with:).

## See Also

### Adding Entries

func addIdentificationEntry(withNextSequentialPhoneNumber: CXCallDirectoryPhoneNumber, label: String)

Adds an identification entry with the specified phone number and label.

