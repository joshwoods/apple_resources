

- Foundation
- NSUnarchiver
-  unarchiveObject(withFile:) Deprecated

Type Method

# unarchiveObject(withFile:)

Decodes and returns the object archived in the file `path`.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func unarchiveObject(withFile path: String) -> Any?
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`path`  

The path to a file than contains an archive created using NSArchiver.

## Return Value

The object, or object graph, that was archived in the file at `path`. Returns `nil` if the file at `path` cannot be unarchived.

## Discussion

This convenience method reads the file by invoking the `NSData` method dataWithContentsOfFile: and then invokes unarchiveObject(with:).

## See Also

### Decoding objects

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object archived in a given `NSData` object.

Deprecated

