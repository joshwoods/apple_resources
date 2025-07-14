

- Contacts
- CNContact
-  isKeyAvailable(\_:) 

Instance Method

# isKeyAvailable(\_:)

Determines whether the contact property value for the specified key is fetched.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func isKeyAvailable(_ key: String) -> Bool
```

## Parameters 

`key`  

A contact property key. For a list of valid keys, see Contact Keys.

## Return Value

true if the value is fetched, otherwise false.

## Discussion

The isKeyAvailable(_:) or areKeysAvailable(_:) methods are used when you are not certain of the keys that were fetched. If this method returns false, refetch the contact using the contact identifier and the keys you want to fetch. Accessing a property that was not fetched will throw CNContactPropertyNotFetchedExceptionName.

## See Also

### Checking the Availability of Data

func areKeysAvailable([any CNKeyDescriptor]) -> Bool

Determines whether all contact property values for the specified keys are fetched.

