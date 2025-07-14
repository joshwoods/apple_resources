

- Contacts
- CNContact
-  areKeysAvailable(\_:) 

Instance Method

# areKeysAvailable(\_:)

Determines whether all contact property values for the specified keys are fetched.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func areKeysAvailable(_ keyDescriptors: [any CNKeyDescriptor]) -> Bool
```

## Parameters 

`keyDescriptors`  

An array of contact property keys and/or key descriptors from contact objects.

## Return Value

true if all the values are fetched; otherwise, false.

## Discussion

The isKeyAvailable(_:) or areKeysAvailable(_:) methods are used where you are not certain of the keys that when fetched. If this method returns false, refetch the contact using the contact identifier and the keys you want to fetch. Accessing a property that was not fetched will throw an CNContactPropertyNotFetchedExceptionName exception.

## See Also

### Checking the Availability of Data

func isKeyAvailable(String) -> Bool

Determines whether the contact property value for the specified key is fetched.

