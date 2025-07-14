

- Core Services
- Carbon Core
- Unicode Utilities
-  UCCreateCollator(\_:\_:\_:\_:) 

Function

# UCCreateCollator(\_:\_:\_:\_:)

Creates an object encapsulating locale and collation information, for the purpose of performing Unicode string comparison.

macOS 10.0+

``` source
func UCCreateCollator(
    _ locale: LocaleRef!,
    _ opVariant: LocaleOperationVariant,
    _ options: UCCollateOptions,
    _ collatorRef: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`locale`  

A valid `LocaleRef` representing a specific locale, or pass `NULL` to request the default system locale. You can supply the value `kUnicodeCollationClass` in the `opClass` parameter of the Locales Utilities functions `LocaleOperationCountLocales` and `LocaleOperationGetLocales` to obtain the locales available for collation on the current system.

`opVariant`  

A `LocaleOperationVariant` value identifying a collation variant within the locale specified in the `locale` parameter. You can also pass 0 to request the default collation variant for any locale. To obtain the varieties of locale-specific collation that are currently available, you can supply the value `kUnicodeCollationClass` in the `opClass` parameter of the Locales Utilities functions `LocaleOperationCountLocales` and `LocaleOperationGetLocales`.

`options`  

A `UCCollateOptions` value specifying any collation options that you want to use for the string comparison.

`collatorRef`  

A pointer to a value of type `CollatorRef`. On return, the `CollatorRef` value contains a valid reference to a new collator object.

## Return Value

A result code. The function can return memory errors and `paramErr`, for example, if the `collatorRef` parameter is `NULL`. It can also return resource errors in Mac OS 9 and CarbonLib.

## Discussion

To perform Unicode string comparison, you must supply locale and collation specifications to a collation function such as UCCompareText(_:_:_:_:_:_:_:). You provide this information by means of a collator object, created via the `UCCreateCollator` function. When finished with the collator object, you dispose of it using the function UCDisposeCollator(_:).

### Special Considerations

The collator object is allocated in the current heap. This function can move memory.

## See Also

### Comparing Unicode Strings

func UCCompareText(CollatorRef!, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses locale-specific collation information to compare Unicode strings.

func UCGetCollationKey(CollatorRef!, UnsafePointer&lt;UniChar>!, Int, Int, UnsafeMutablePointer&lt;Int>!, UnsafeMutablePointer&lt;UCCollationValue>!) -> OSStatus

Uses locale-specific collation information to generate a collation key for a Unicode string.

func UCCompareCollationKeys(UnsafePointer&lt;UCCollationValue>!, Int, UnsafePointer&lt;UCCollationValue>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses collation keys to compare Unicode strings.

func UCDisposeCollator(UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Disposes a collator object.

func UCCompareTextDefault(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses the default system locale to compare Unicode strings.

func UCCompareTextNoLocale(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses a fixed, locale-insensitive order to compare Unicode strings.

