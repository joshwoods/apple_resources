

- Foundation
- NSArchiver
-  encodeClassName(\_:intoClassName:) Deprecated

Instance Method

# encodeClassName(\_:intoClassName:)

Encodes a substitute name for the class with a given true name.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func encodeClassName(
    _ trueName: String,
    intoClassName inArchiveName: String
)
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`trueName`  

The real name of a class in the object graph being archived.

`inArchiveName`  

The name of the class to use in the archive in place of `trueName`.

## Discussion

Any subsequently encountered objects of class `trueName` are archived as instances of class `inArchiveName`. It is safest not to invoke this method during the archiving process (that is, within an encode(with:) method). Instead, invoke it before encodeRootObject(_:).

## See Also

### Substituting classes or objects

func classNameEncoded(forTrueClassName: String) -> String?

Returns the name of the class used to archive instances of the class with a given true name.

Deprecated

func replace(Any, with: Any)

Causes the receiver to treat subsequent requests to encode a given object as though they were requests to encode another given object.

Deprecated

