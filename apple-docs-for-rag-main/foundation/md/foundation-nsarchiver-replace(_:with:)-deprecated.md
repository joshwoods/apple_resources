

- Foundation
- NSArchiver
-  replace(\_:with:) Deprecated

Instance Method

# replace(\_:with:)

Causes the receiver to treat subsequent requests to encode a given object as though they were requests to encode another given object.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func replace(
    _ object: Any,
    with newObject: Any
)
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`object`  

An object in the object graph being archived.

`newObject`  

The object with which to replace `object` in the archive.

## Discussion

Both `object` and `newObject` must be valid objects.

## See Also

### Substituting classes or objects

func classNameEncoded(forTrueClassName: String) -> String?

Returns the name of the class used to archive instances of the class with a given true name.

Deprecated

func encodeClassName(String, intoClassName: String)

Encodes a substitute name for the class with a given true name.

Deprecated

