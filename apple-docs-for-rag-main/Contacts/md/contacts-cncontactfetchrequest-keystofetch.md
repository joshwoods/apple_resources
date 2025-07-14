

- Contacts
- CNContactFetchRequest
-  keysToFetch 

Instance Property

# keysToFetch

The properties to fetch in the returned contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var keysToFetch: [any CNKeyDescriptor] { get set }
```

## Discussion

An array of contact property keys or key descriptors from contact objects to be fetched in the returned contacts. For example, CNContactEmailAddressesKey, CNContactPhoneNumbersKey, CNContactFormatterStyle.fullName fetches the contact’s email addresses, phone numbers, and contact’s full name with the contact formatter.

