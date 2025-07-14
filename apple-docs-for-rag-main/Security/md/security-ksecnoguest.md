

- Security
-  kSecNoGuest 

Global Variable

# kSecNoGuest

Not a valid `SecGuestRef` object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecNoGuest: SecGuestRef { get }
```

## Discussion

Some functions in the API use this value to indicate that there is no guest, and some functions use it to indicate that the function applies to the host itself rather than to a guest.

