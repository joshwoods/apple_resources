

- Foundation
- NSUnarchiver
-  replace(\_:with:) Deprecated

Instance Method

# replace(\_:with:)

Causes the receiver to substitute one given object for another whenever the latter is extracted from the archive.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func replace(
    _ object: Any,
    with newObject: Any
)
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`object`  

The archived object to replace.

`newObject`  

The object with which to replace `object`.

## Discussion

`newObject` can be of a different class from object, and the class mappings set by classNameDecoded(forArchiveClassName:) and decodeClassName(_:asClassName:) are ignored.

## See Also

### Substituting classes or objects

class func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class used when instantiating objects whose ostensible class, according to the archived data, is a given name.

Deprecated

class func decodeClassName(String, asClassName: String)

Instructs instances of `NSUnarchiver` to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

Deprecated

func classNameDecoded(forArchiveClassName: String) -> String

Returns the name of the class that will be used when instantiating objects whose ostensible class, according to the archived data, is a given name.

Deprecated

func decodeClassName(String, asClassName: String)

Instructs the receiver to use the class with a given name when instantiating objects whose ostensible class, according to the archived data, is another given name.

Deprecated

