

- CallKit
- CXCallDirectoryExtensionContext
-  addIdentificationEntry(withNextSequentialPhoneNumber:label:) 

Instance Method

# addIdentificationEntry(withNextSequentialPhoneNumber:label:)

Adds an identification entry with the specified phone number and label.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func addIdentificationEntry(
    withNextSequentialPhoneNumber phoneNumber: CXCallDirectoryPhoneNumber,
    label: String
)
```

## Parameters 

`phoneNumber`  

The phone number to be identified.

`label`  

The label to identify the phone number.

## Mentioned in 

Identifying and blocking calls

## Discussion

When a phone number has an identification entry, incoming calls from that phone number will display its associated label to the user.

Call this method on the instance of CXCallDirectoryExtensionContext passed as an argument to the block parameter of the CXCallDirectoryProvider instance method beginRequest(with:).

## See Also

### Adding Entries

func addBlockingEntry(withNextSequentialPhoneNumber: CXCallDirectoryPhoneNumber)

Adds a blocking entry with the specified phone number.

