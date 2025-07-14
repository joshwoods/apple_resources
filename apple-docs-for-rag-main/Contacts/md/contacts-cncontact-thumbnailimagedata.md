

- Contacts
- CNContact
-  thumbnailImageData 

Instance Property

# thumbnailImageData

The thumbnail version of the contact’s profile picture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var thumbnailImageData: Data? { get }
```

## Discussion

The thumbnailImageData property is derived from the imageData property, including cropping information from vCards or edits from contact viewing. It is recommended that you fetch this property only when you need to access its value, such as when you need to display the contact’s profile thumbnail picture.

## See Also

### Getting Contact Images

var imageData: Data?

The profile picture of a contact.

var imageDataAvailable: Bool

A Boolean indicating whether a contact has a profile picture.

