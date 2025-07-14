

- UIKit
-  UIPasteboard 

Class

# UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIPasteboard
```

## Overview

For sharing data with any other app, use the systemwide general pasteboard. For sharing data with another app from your team — that has the same team ID as the app to share from — configure an App Group. For more information about configuring an App Group, see Configuring app groups.

In typical usage, an object in your app writes data to a pasteboard when the user requests a copy, cut, or duplicate operation on a selection in the user interface. Another object in the same or different app then reads that data from the pasteboard and presents it to the user at a new location. This usually happens when the user requests a paste operation.

Important

Starting in iOS 14, the system notifies the user when an app gets general pasteboard content that originates in a different app without *user intent*. The system determines user intent based on user interactions, such as tapping a system-provided control or pressing Command-V. Use the properties and methods below to determine whether pasteboard items match various patterns, such as web search terms, URLs, or numbers, without notifying the user.

### The general pasteboard and named pasteboards

The system identifies the systemwide general pasteboard with the general pasteboard name, and you can use it for any type of data. Obtain the general pasteboard from the general shared system pasteboard object.

You can create named pasteboards with the class methods init(name:create:) and withUniqueName() for sharing data within your app, and from your app to other apps that have the same Team ID.

### Using pasteboards

The UIPasteboard class provides methods for reading and writing individual pasteboard items, as well as methods for reading and writing multiple pasteboard items at once. For more information, see Getting and setting pasteboard items in the topic groups below. The data to write to a pasteboard can be in one of the following forms:

- If the data is an object that conforms to NSItemProviderWriting, use setItemProviders(_:localOnly:expirationDate:) to write it to the pasteboard.

- If you can represent the data with a common object — such as NSString, NSArray, NSDictionary, NSDate, NSNumber, UIImage, or NSURL — you can write it to the pasteboard as a value using a method such as setValue(_:forPasteboardType:).

- If the data is binary, use the setData(_:forPasteboardType:) method to write it to the pasteboard.

The UIPasteboard class provides convenience methods for writing and reading strings, images, URLs, and colors to and from single or multiple pasteboard items. See Getting and setting pasteboard items of standard data types in the topic groups below.

Note

Before you attempt to read a particular data type from a pasteboard by using the methods in Getting and setting pasteboard items of standard data types in the topic groups below, check for the presence of data of the type you want. Do this by using the type-checking methods.

UIPasteboard provides properties for directly checking whether specific data types are present on a pasteboard, see Checking for data types on a pasteboard in the topic groups below. Use these properties, rather than attempting to read pasteboard data, to avoid causing the system to needlessly attempt to fetch data before necessary, or when the data might not be present. For example, use the hasStrings property to determine whether to present a string-data paste option in the user interface, using code like the following:

```
if UIPasteboard.general.hasStrings {
    // Enable string-related control...
}
```

Use the following properties to avoid user notifications and alerts when the system doesn’t establish user intent:

- numberOfItems

- types, types(forItemSet:)

- itemSet(withPasteboardTypes:)

- hasColors, hasImages, hasStrings, hasURLs

- canLoadObject(ofClass:), canLoadObject(ofClass:)

- any of the pattern-detection methods in the Detecting patterns of content in pasteboard items group in the topic groups below

The system notifies the user when you access properties or call methods that pull data from the pasteboard if the system doesn’t determine that the user intends to access that data.

### Pasteboard items and representation types

When you write an object to a pasteboard, the pasteboard stores it as a *pasteboard item*. A pasteboard item consists of one or more key-value pairs in which the key identifies the representation type (sometimes called a *pasteboard type*) of the value.

A uniform type identifier frequently functions as the key for a representation type. For example, you can use the UTTypeJPEG uniform type identifier (a constant for `public.jpeg`) as a representation type key for JPEG data.

For a discussion of uniform type identifiers, and a list of common ones, see Uniform Type Identifiers.

Your app can use any string to name a representation type; however, for app-specific data types, it’s best practice to use reverse-DNS notation to ensure the uniqueness of the type (for example, `com.myCompany.myApp.myType`).

You can provide flexibility for data sharing by providing multiple representation types for a pasteboard item during a copy or cut operation. Various contexts within your app or other apps can then make use of an appropriate representation type. For example, when a user copies an image, your app can write multiple representation types, such as in the PNG, JPEG, and GIF data formats, to a pasteboard. If the original image is in PNG format, but the receiving app can handle only GIF images, it can still use the pasteboard data.

For more about representation types, read the discussion for the types instance method.

### Sharing pasteboards between devices

When a user signs into iCloud, the general pasteboard automatically transfers its contents to nearby devices that use the same iCloud account. You can control Handoff behavior when writing contents to the general pasteboard, and can set an expiration for items, using the setItemProviders(_:localOnly:expirationDate:), setObjects(_:localOnly:expirationDate:), or setItems(_:options:) methods, as follows:

- To exclude a pasteboard from Handoff, specify false for the `localOnly` parameter, or call the setItems(_:options:) method with the localOnly option.

- To indicate an expiration time and date for copied data, provide the `expirationDate` parameter, or call the setItems(_:options:) method with the expirationDate option. At the time and date that you set, the system removes the pasteboard items from the pasteboard.

### Using pasteboards with other objects

Although the UIPasteboard class is central to copy, paste, and duplicate operations, you can employ protocols and instances of other UIKit classes in these operations as well, such as the following:

- UIEditMenuInteraction — Displays a menu with edit actions, such as Copy, Cut, Paste, Select, and Select All, above or below the selection.

- UIActivityItemsConfigurationReading — Objects implement this protocol to indicate that they support copying and sharing data.

- UIPasteConfigurationSupporting — Objects implement this protocol to indicate whether they support pasting with a specific UIPasteConfiguration.

- UIResponder — Responders implement canPerformAction(_:withSender:) to enable or disable commands in the above-mentioned menu based on the current context.

- UIResponderStandardEditActions — Responders implement methods that this informal protocol declares to handle the chosen menu commands (for example, `copy:` and `paste:`).

A typical app that implements copy, paste, and duplicate operations also manages and presents related selections in its user interface. In addition, your app needs to coordinate changes in pasteboard content with changes to its data model, as appropriate for your app.

## Topics

### Getting and removing pasteboards

class var general: UIPasteboard

The systemwide general pasteboard, which you use for general copy-paste operations.

init?(name: UIPasteboard.Name, create: Bool)

Returns a pasteboard that you identify by name, optionally creating it if it doesn’t exist.

class func withUniqueName() -> UIPasteboard

Returns an app pasteboard that you identify by a unique system-generated name.

class func remove(withName: UIPasteboard.Name)

Invalidates the designated app pasteboard.

### Getting and setting pasteboard attributes

var name: UIPasteboard.Name

The name of the pasteboard.

var changeCount: Int

The number of times the pasteboard’s contents change.

### Detecting patterns of content in pasteboard items

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard, and return the patterns that it matches.

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>], any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard items, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>]

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard items, and return the patterns that it matches.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;UIPasteboard.DetectedValues, any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard, and provide the values that it matches to your closure.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> UIPasteboard.DetectedValues

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard, and return the values that it matches.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[UIPasteboard.DetectedValues], any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard items, and provide the values that it matches to your closure.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [UIPasteboard.DetectedValues]

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard item, and return the values that it matches for each pasteboard.

struct DetectedValues

An object that contains common types of data that the data detection system matches for a pasteboard.

struct DetectionPattern

An object that represents a pattern to detect for the pasteboard, such as a URL, text, or a number.

### Determining types of pasteboard items

var types: [String]

The types of the first item on the pasteboard.

func types(forItemSet: IndexSet?) -> [[String]]?

Returns an array of representation types for each specified pasteboard item.

func contains(pasteboardTypes: [String]) -> Bool

Returns whether the pasteboard holds data of the specified representation type.

func contains(pasteboardTypes: [String], inItemSet: IndexSet?) -> Bool

Returns whether the specified pasteboard items contain data of the given representation types.

func itemSet(withPasteboardTypes: [String]) -> IndexSet?

Returns an index set identifying pasteboard items having the specified representation types.

### Getting and setting pasteboard items

var numberOfItems: Int

The number of items for the pasteboard.

var items: [[String : Any]]

The pasteboard items on the pasteboard.

func addItems([[String : Any]])

Appends pasteboard items to the current contents of the pasteboard.

func setItems([[String : Any]], options: [UIPasteboard.OptionsKey : Any])

Adds an array of items to a pasteboard, and sets privacy options for all the items on the pasteboard.

func data(forPasteboardType: String) -> Data?

Returns the data on the pasteboard for the given representation type.

func data(forPasteboardType: String, inItemSet: IndexSet?) -> [Data]?

Returns the data objects in the indicated pasteboard items that have the given representation type.

func setData(Data, forPasteboardType: String)

Puts data on the pasteboard for the specified representation type.

func value(forPasteboardType: String) -> Any?

Returns an object on the pasteboard for the given representation type.

func values(forPasteboardType: String, inItemSet: IndexSet?) -> [Any]?

Returns the objects on the indicated pasteboard items that have the given representation type.

func setValue(Any, forPasteboardType: String)

Puts an object on the pasteboard for the specified representation type.

### Getting and setting pasteboard items of standard data types

var string: String?

The string value of the first pasteboard item.

var strings: [String]?

An array of strings in all pasteboard items.

var image: UIImage?

The image object of the first pasteboard item.

var images: [UIImage]?

An array of image objects in all pasteboard items.

var url: URL?

The URL object of the first pasteboard item.

var urls: [URL]?

An array of URL objects in all pasteboard items.

var color: UIColor?

The color object of the first pasteboard item.

var colors: [UIColor]?

An array of color objects in all pasteboard items.

### Checking for data types on a pasteboard

var hasColors: Bool

A Boolean value that indicates whether the pasteboard contains contains a nonempty array of colors.

var hasImages: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of images.

var hasStrings: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of strings.

var hasURLs: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of URLs.

### Getting and setting item providers

var itemProviders: [NSItemProvider]

An array of item providers for the pasteboard.

func setItemProviders([NSItemProvider], localOnly: Bool, expirationDate: Date?)

Sets and configures an explicit array of item providers for the pasteboard.

func setObjects([any NSItemProviderWriting])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects([any NSItemProviderWriting], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

### Constants

struct Name

Constants that identify the name of a pasteboard.

Pasteboard Names

Names identifying the system pasteboards.

struct OptionsKey

Options for describing pasteboard privacy.

Pasteboard Data Type Representations

Pasteboard-item representation types, as for a given object value.

UserInfo Dictionary Keys

Use these keys to access the representation types of pasteboard items that you add to, or remove from, a pasteboard.

### Notifications

class let changedNotification: NSNotification.Name

A notification that a pasteboard object posts when its contents change.

class let removedNotification: NSNotification.Name

A notification that a pasteboard object posts just before an app removes it.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

