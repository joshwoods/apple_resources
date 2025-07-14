

- Core Services
- Carbon Core
- Unicode Utilities
-  UCGetCollationKey(\_:\_:\_:\_:\_:\_:) 

Function

# UCGetCollationKey(\_:\_:\_:\_:\_:\_:)

Uses locale-specific collation information to generate a collation key for a Unicode string.

macOS 10.0+

``` source
func UCGetCollationKey(
    _ collatorRef: CollatorRef!,
    _ textPtr: UnsafePointer!,
    _ textLength: Int,
    _ maxKeySize: Int,
    _ actualKeySize: UnsafeMutablePointer!,
    _ collationKey: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`collatorRef`  

A valid reference to a collator object; `NULL` is not allowed. You can use the function UCCreateCollator(_:_:_:_:) to obtain a collator reference.

`textPtr`  

A pointer to the Unicode string (a `UniChar` array) for which to generate a collation key.

`textLength`  

The total count of Unicode characters in the string referenced by the `textPtr` parameter.

`maxKeySize`  

An `ItemCount` value specifying the length of the `UCCollationValue` array passed in the `collationKey` parameter. This dimension should typically be at least `5*textLength`, as the byte length of a collation key is typically more than 16 times the number of Unicode characters in the string.

`actualKeySize`  

On return, the actual length of the `UCCollationValue` array returned in the `collationKey` parameter.

`collationKey`  

An array of `UCCollationValue` values. On return, the array contains the new collation key. The collation key consists of a sequence of primary weights for all of the collation text elements in the string, followed by a separator and a sequence of secondary weights for all of the text elements in the string, and so on for several levels of significance. The separator is usually 0; however, 1 is used as the separator at the boundary between levels that are significant and levels that are insignificant for the options you supply in the collator object.

## Return Value

A result code. The function can return `paramErr`, for example, if the parameters `collatorRef`, `textPtr`, `actualKeySize`, or `collationKey` are `NULL`. It can also return memory errors. If `maxKeySize` is too small for the collation key, the function returns `kUCOutputBufferTooSmall`.

## Discussion

If you want to compare the same strings several times, as when sorting a list of strings, it may be most efficient for you to derive a collation key for each string and then compare the collation keys. A collation key is a transformation of the string that depends on the collator object (that is, it depends on the locale, the collation variant if any, and the collation options).

Collation keys that are generated using the same collator object—but for different strings—can quickly be compared with each other, without further reference to the collator object or collation tables. The disadvantage is that the collation keys may be rather large. After you use the `UCGetCollationKey` function to create a collation key from a given string and collator object, you can call the function UCCompareCollationKeys(_:_:_:_:_:_:) to compare two collation keys that were generated with the same collator object.

If you are comparing different strings, it may be more efficient for you to call the function UCCompareText(_:_:_:_:_:_:_:) multiple times using the same collator object.

Note that collation keys should be used only in a runtime context. They should not be stored in a persistent state (such as to disk) because the format of a collation key could change in the future.

### Special Considerations

This function can move memory.

## See Also

### Comparing Unicode Strings

func UCCreateCollator(LocaleRef!, LocaleOperationVariant, UCCollateOptions, UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Creates an object encapsulating locale and collation information, for the purpose of performing Unicode string comparison.

func UCCompareText(CollatorRef!, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses locale-specific collation information to compare Unicode strings.

func UCCompareCollationKeys(UnsafePointer&lt;UCCollationValue>!, Int, UnsafePointer&lt;UCCollationValue>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses collation keys to compare Unicode strings.

func UCDisposeCollator(UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Disposes a collator object.

func UCCompareTextDefault(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses the default system locale to compare Unicode strings.

func UCCompareTextNoLocale(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses a fixed, locale-insensitive order to compare Unicode strings.

