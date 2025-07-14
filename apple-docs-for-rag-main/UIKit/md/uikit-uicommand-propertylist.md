

- UIKit
- UICommand
-  propertyList 

Instance Property

# propertyList

An object that contains data to associate with the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var propertyList: Any? { get }
```

## Discussion

Use propertyList to associate a small amount of data to the command.

- Swift
- Objective-C

In Swift, the property list should contain only standard library types such as Array, Dictionary, String, Int, and Double, and Foundation types such as Date and Data.

In Objective-C, the property list should contain only NSArray, NSDictionary, NSString, NSNumber, NSDate, and NSData objects.

## See Also

### Associating data

let UICommandTagShare: String

A value that identifies a command as a Share menu.

