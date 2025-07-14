

- Core Services
- Carbon Core
- Unicode Utilities
-  UCCompareTextNoLocale(\_:\_:\_:\_:\_:\_:\_:) 

Function

# UCCompareTextNoLocale(\_:\_:\_:\_:\_:\_:\_:)

Uses a fixed, locale-insensitive order to compare Unicode strings.

macOS 10.0+

``` source
func UCCompareTextNoLocale(
    _ options: UCCollateOptions,
    _ text1Ptr: UnsafePointer!,
    _ text1Length: Int,
    _ text2Ptr: UnsafePointer!,
    _ text2Length: Int,
    _ equivalent: UnsafeMutablePointer!,
    _ order: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`options`  

A `UCCollateOptions` value specifying the fixed ordering scheme to use for the string comparison. This value must be nonzero. Bits 24-31 of `UCCollateOptionsValue` specify which fixed ordering scheme to use. Currently there is only scheme—`kUCCollateTypeHFSExtended`. See Fixed Ordering Scheme for additional details.

`text1Ptr`  

A pointer to the first Unicode string (a `UniChar` array) to compare.

`text1Length`  

The total count of Unicode characters in the first string being compared.

`text2Ptr`  

A pointer to the second Unicode string to compare.

`text2Length`  

The total count of Unicode characters in the second string being compared.

`equivalent`  

A pointer to a `Boolean` value or pass `NULL`. On return, `UCCompareTextNoLocale` produces a value of `true` if the strings are equivalent for the ordering scheme you have specified. If you wish simply to sort a list of strings in order, using the specified ordering scheme, you can pass `NULL` for the `equivalent` parameter and only use the `order` parameter’s result. In this case, all available comparison criteria are used to put the strings in a deterministic order, even if they are considered “equivalent” for the specified ordering scheme. Note that you can set either the `equivalent` or the `order` parameters to `NULL`, but not both.

`order`  

A pointer to a signed, 32-bit integer value, or pass `NULL`. If you wish simply to test the strings for equivalence, using the specified ordering scheme (which can be much faster than determining ordering), you can pass `NULL` for the `order` parameter and only use the `equivalent` parameter’s result. (Note that either the `equivalent` or the `order` parameters may be `NULL`, but not both.

## Return Value

A result code. This function can return `paramErr` if you pass an invalid value for one of the parameters. For example, if you pass `0` for the `options` paramter, the function returns `paramErr`.

## Discussion

You can call the `UCCompareTextNoLocale` function when you want to perform a fixed, locale-insensitive comparison that is guaranteed not to change from one system release to the next. This type of comparison could be used for sorting a Unicode key string in a database, for example. The `UCCompareTextNoLocale` function can provide comparison according to various fixed ordering schemes (only one is supported for Mac OS 8.6 and 9.0). This type of comparison is not usually used for a user-visible ordering, so the ordering schemes need not match any user’s expectation of a sensible collation order.

The `UCCompareTextNoLocale` function does not require a collator object or collation keys. Another advantage of `UCCompareTextNoLocale` on Mac OS 9 is that it is exported from the `UnicodeUtilitiesCoreLib` library, which does not depend on other libraries (the other comparison functions exported from `UnicodeUtilitiesLib`, which depends on `LocalesLib` and `TextCommon`).

## See Also

### Comparing Unicode Strings

func UCCreateCollator(LocaleRef!, LocaleOperationVariant, UCCollateOptions, UnsafeMutablePointer&lt;CollatorRef?>!) -> OSStatus

Creates an object encapsulating locale and collation information, for the purpose of performing Unicode string comparison.

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

