

- Wallet Passes
-  Pass 

Object

# Pass

An object that represents a pass.

iOS 6.0+iPadOS 6.0+watchOS 2.0+

``` source
object Pass
```

## Properties

`accessibilityURL`

`string`

A URL that links to your accessiblity content, or the venue’s.

This key works only for poster event tickets.

`addOnURL`

`string`

A URL that can link to experiences that someone can add to the pass.

This key works only for poster event tickets.

`appLaunchURL`

`string`

A URL the system passes to the associated app from `associatedStoreIdentifiers` during launch.

The app receives this URL in the application(_:didFinishLaunchingWithOptions:) and application(_:open:options:) methods of its app delegate.

This key isn’t supported for watchOS.

`associatedStoreIdentifiers`

`[number]`

An array of App Store identifiers for apps associated with the pass. The associated app on a device is the first item in the array that’s compatible with that device.

A link to launch the app is on the back of the pass. If the app isn’t installed, the link opens the App Store.

This key works only for payment passes.

This key isn’t supported for watchOS.

`auxiliaryStoreIdentifiers`

`[number]`

An array of additional App Store identifiers for apps associated with the pass. The associated app on a device is the first item in the array that’s compatible with that device.

This key works only for poster event tickets. A link to launch the app is in the event guide of the pass. If the app isn’t installed, the link opens the App Store.

This key isn’t supported for watchOS.

`authenticationToken`

`string`

The authentication token to use with the web service in the `webServiceURL` key.

`backgroundColor`

`string`

A background color for the pass, specified as a CSS-style RGB triple, such as `rgb(23, 187, 82)`.

`bagPolicyURL`

`string`

A URL that links to the bag policy of the venue for the event that the pass represents.

This key works only for poster event tickets.

`barcode`

Pass.Barcode

An object that represents a barcode on a pass.

This object is deprecated. Use `barcodes` instead.

`barcodes`

`[`Pass.Barcodes`]`

An array of objects that represent possible barcodes on a pass. The system uses the first displayable barcode for the device.

`beacons`

`[`Pass.Beacons`]`

An array of objects that represent the identity of Bluetooth Low Energy beacons the system uses to show a relevant pass.

`boardingPass`

Pass.BoardingPass

An object that contains the information for a boarding pass.

`contactVenueEmail`

`string`

The preferred email address to contact the venue, event, or issuer.

This key works only for poster event tickets.

`contactVenuePhoneNumber`

`string`

The phone number for contacting the venue, event, or issuer.

This key works only for poster event tickets.

`contactVenueWebsite`

`string`

A URL that links to the website of the venue, event, or issuer.

This key works only for poster event tickets.

`coupon`

Pass.Coupon

An object that contains the information for a coupon.

`description`

`localizable string`

 (Required) 

A short description that iOS accessibility technologies use for a pass.

`directionsInformationURL`

`string`

A URL that links to directions for the event.

This key works only for poster event tickets.

`eventLogoText`

`localizable string`

The text to display next to the logo on the pass.

This key works only for poster event tickets

`eventTicket`

Pass.EventTicket

An object that contains the information for an event ticket.

`expirationDate`

`string`

The date and time the pass expires. The value needs to be a complete date that includes hours and minutes, and may optionally include seconds.

`footerBackgroundColor`

`string`

A background color for the footer of the pass, specified as a CSS-style RGB triple, such as `rgb(100, 10, 110)`.

This key works only for poster event tickets.

`foregroundColor`

`string`

A foreground color for the pass, specified as a CSS-style RGB triple, such as `rgb(100, 10, 110)`.

`formatVersion`

`number`

 (Required) 

The version of the file format. The value needs to be `1`.

`generic`

Pass.Generic

An object that contains the information for a generic pass.

`groupingIdentifier`

`string`

An identifier the system uses to group related boarding passes or event tickets. Wallet displays passes with the same `groupingIdentifier`, `passTypeIdentifier`, and type as a group.

Use this identifier to group passes that are tightly related, such as boarding passes for different connections on the same trip.

`labelColor`

`string`

A color for the label text of the pass, specified as a CSS-style RGB triple, such as `rgb(100, 10, 110)`. If you don’t provide a value, the system determines the label color.

`locations`

`[`Pass.Locations`]`

An array of up to 10 objects that represent geographic locations the system uses to show a relevant pass.

`logoText`

`localizable string`

The text to display next to the logo on the pass.

This key doesn’t work for poster event tickets.

`maxDistance`

`number`

The maximum distance, in meters, from a location in the `locations` array at which the pass is relevant. The system uses the smaller of this distance or the default distance.

`merchandiseURL`

`string`

A URL that links to a site for ordering merchandise for the event that the pass represents.

This key works only for poster event tickets.

`nfc`

Pass.NFC

An object that contains the information to use for Value-Added Services protocol transactions.

`orderFoodURL`

`string`

A URL that links to the food ordering page for the event that the pass represents.

This key works only for poster event tickets.

`organizationName`

`localizable string`

 (Required) 

The name of the organization.

`parkingInformationURL`

`string`

A URL that links to parking information for the event that the pass represents.

This key works only for poster event tickets.

`passTypeIdentifier`

`string`

 (Required) 

The pass type identifier that’s registered with Apple. The value needs to be the same as the distribution certificate that signs the pass.

`preferredStyleSchemes`

`[string]`

An array of schemes to validate the pass with. The system validates the pass and its contents to ensure they meet the schemes’ requirements, falling back to the designed type if validation fails for all the provided schemes.

`purchaseParkingURL`

`string`

A URL that links to a site to purchase parking for the event that the pass represents.

This key works only for poster event tickets.

`relevantDate`

`string`

The date and time when the pass becomes relevant, as a W3C timestamp, such as the start time of a movie. The value needs to be a complete date that includes hours and minutes, and may optionally include seconds.

For information about the W3C timestamp format, see Time and Date Formats on the W3C website.

This object is deprecated. Use `relevantDates` instead.

`relevantDates`

`[`Pass.RelevantDates`]`

An array of objects that represent date intervals that the system uses to show a relevant pass.

`sellURL`

`string`

A URL that links to the selling flow for the ticket the pass represents.

This key works only for poster event tickets.

`semantics`

SemanticTags

An object that contains machine-readable metadata the system uses to offer a pass and suggest related actions. For example, setting Don’t Disturb mode for the duration of a movie.

`serialNumber`

`string`

 (Required) 

An alphanumeric serial number. The combination of the serial number and pass type identifier needs to be unique for each pass.

`sharingProhibited`

`boolean`

A Boolean value introduced in iOS 11 that controls whether to show the Share button on the back of a pass. A value of `true` removes the button. The default value is `false`. This flag has no effect in earlier versions of iOS, nor does it prevent sharing the pass in some other way.

`storeCard`

Pass.StoreCard

An object that contains the information for a store card.

`suppressStripShine`

`boolean`

A Boolean value that controls whether to display the strip image without a shine effect. The default value is `true`.

`suppressHeaderDarkening`

`boolean`

A Boolean value that controls whether to display the header darkening gradient on poster event tickets. The default value is `false`.

This key works only for poster event tickets.

`teamIdentifier`

`string`

 (Required) 

The Team ID for the Apple Developer Program account that registered the pass type identifier.

`transferURL`

`string`

A URL that links to the transferring flow for the ticket that the pass represents.

This key works only for poster event tickets.

`transitInformationURL`

`string`

A URL that links to information about transit options in the area of the event that the pass represents.

This key works only for poster event tickets.

`useAutomaticColors`

`boolean`

A Boolean value that controls whether Wallet computes the foreground and label color that the pass uses. The system derives the background color from the background image of the pass.

This key works only for poster event tickets.

This key ignores the values that `foregroundColor` and `labelColor` specify.

`userInfo`

`any JSON data`

A JSON dictionary that contains any custom information for companion apps. The data doesn’t appear to the user.

For example, a pass for a cafe might include information about the customer’s favorite drink and sandwich in a machine-readable form. The companion app uses the data for placing an order for *the usual*.

`voided`

`boolean`

A Boolean value that indicates that the pass is void, such as a redeemed, one-time-use coupon. The default value is `false`.

`webServiceURL`

`string`

The URL for a web service that you use to update or personalize the pass. The URL can include an optional port number.

## Mentioned in 

Supporting semantic tags in Wallet passes

Showing a Pass on the Lock Screen

Distributing and updating a pass

Building a Pass

Adding a Web Service to Update Passes

## Topics

### Setting the pass type

object Pass.BoardingPass

An object that represents the groups of fields that display the information for a boarding pass.

object Pass.Coupon

An object that represents the groups of fields that display the information for a coupon.

object Pass.EventTicket

An object that represents the groups of fields that display the information for an event ticket.

object Pass.Generic

An object that represents the groups of fields that display the information for a generic pass.

### Adding content

object PassFields

An object that represents the groups of fields that display information on the front and back of a pass.

object PassFieldContent

An object that represents the information to display in a field on a pass.

### Adding system suggestions

Supporting semantic tags in Wallet passes

Enable the system to offer suggestions for actions related to passes by adding machine-readable metadata.

object SemanticTags

An object that contains machine-readable metadata the system uses to offer a pass and suggest related actions.

object SemanticTagType

A compilation of data object types for semantic tags.

### Adding barcodes

object Pass.Barcodes

An object that represents a barcode on a pass.

object Pass.Barcode

An object that represents a barcode shown on a pass.

Deprecated

### Adding relevance

Showing a Pass on the Lock Screen

Add information to your pass so the system can display it on the Lock Screen at a relevant time and place.

object Pass.Locations

An object that represents a location that the system uses to show a relevant pass.

object Pass.Beacons

An object that represents the identifier of a Bluetooth Low Energy beacon the system uses to show a relevant pass.

object Pass.RelevantDates

An object that represents a date interval that the system uses to show a relevant pass.

### Adding near-field communications

object Pass.NFC

An object that represents the near-field communication (NFC) payload the device passes to an Apple Pay terminal.

### Adding personalization information

object Pass.StoreCard

An object that represents groups of fields that show the information for a store card.

object Personalize

An object that contains the personalization information for a rewards pass.

## See Also

### Essentials

Creating the Source for a Pass

Create the directory structure and add source files and images to define a pass.

Building a Pass

Build a distributable pass.

Distributing and updating a pass

Distribute a pass to your users or update an existing pass.

