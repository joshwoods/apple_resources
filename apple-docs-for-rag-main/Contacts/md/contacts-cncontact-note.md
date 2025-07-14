

- Contacts
- CNContact
-  note 

Instance Property

# note

A string containing notes for the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var note: String { get }
```

## Mentioned in 

Accessing the contact store

## Discussion

To fetch the `note` property in iOS 13 or later or macOS 13 or later, add the com.apple.developer.contacts.notes entitlement to your app. The entitlement requires permission from Apple to use, and you can’t publicly distribute your app until you have permission to use it. For more information about adding the entitlement and getting permission, see com.apple.developer.contacts.notes.

