

- Foundation
- NSUnarchiver
-  classNameDecoded(forArchiveClassName:) Deprecated

Type Method

# classNameDecoded(forArchiveClassName:)

Returns the name of the class used when instantiating objects whose ostensible class, according to the archived data, is a given name.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func classNameDecoded(forArchiveClassName inArchiveName: String) -> String
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`inArchiveName`  

The name of a class.

## Return Value

The name of the class used when instantiating objects whose ostensible class, according to the archived data, is `nameInArchive`. Returns `nameInArchive` if no substitute name has been specified using the class method (not the instance method) decodeClassName(_:asClassName:).

## Discussion

Note that each individual instance of `NSUnarchiver` can be given its own class name mappings by invoking the instance method decodeClassName(_:asClassName:). The `NSUnarchiver` class has no information about these instance-specific mappings, however, so they don’t affect the return value of classNameDecoded(forArchiveClassName:).

## See Also

### Substituting classes or objects

class func decodeClassName(String, asClassName: String)

Instructs instances of `NSUnarchiver` to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

Deprecated

func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class that will be used when instantiating objects whose ostensible class, according to the archived data, is a given name.

Deprecated

func decodeClassName(String, asClassName: String)

Instructs the receiver to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

Deprecated

func replace(Any, with: Any)

Causes the receiver to substitute one given object for another whenever the latter is extracted from the archive.

Deprecated

