

- Contacts
- CNContact
-  imageData 

Instance Property

# imageData

The profile picture of a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var imageData: Data? { get }
```

## Discussion

It is recommended that you fetch this property only when you need to access its value, such as when you need to display the contact’s profile picture.

## See Also

### Getting Contact Images

var thumbnailImageData: Data?

The thumbnail version of the contact’s profile picture.

var imageDataAvailable: Bool

A Boolean indicating whether a contact has a profile picture.

