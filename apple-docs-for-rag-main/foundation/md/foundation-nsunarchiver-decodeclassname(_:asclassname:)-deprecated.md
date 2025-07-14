

- Foundation
- NSUnarchiver
-  decodeClassName(\_:asClassName:) Deprecated

Type Method

# decodeClassName(\_:asClassName:)

Instructs instances of `NSUnarchiver` to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func decodeClassName(
    _ inArchiveName: String,
    asClassName trueName: String
)
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`inArchiveName`  

The ostensible name of a class in an archive.

`trueName`  

The name of the class to use when instantiating objects whose ostensible class, according to the archived data, is `nameInArchive`.

## Discussion

This method enables easy conversion of unarchived data when the name of a class has changed since the archive was created.

Note that there is also an instance method of the same name. An instance of `NSUnarchiver` can maintain its own mapping of class names. However, if both the class method and the instance method have been invoked using an identical value for `nameInArchive`, the class method takes precedence.

## See Also

### Substituting classes or objects

class func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class used when instantiating objects whose ostensible class, according to the archived data, is a given name.

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

