

- Core Services
- Carbon Core
- Unicode Utilities
-  UCCompareTextDefault(\_:\_:\_:\_:\_:\_:\_:) 

Function

# UCCompareTextDefault(\_:\_:\_:\_:\_:\_:\_:)

Uses the default system locale to compare Unicode strings.

macOS 10.0+

``` source
func UCCompareTextDefault(
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

A `UCCollateOptions` value specifying any collation options for the string comparison.

`text1Ptr`  

A pointer to the first Unicode string (a `UniChar` array) to compare.

`text1Length`  

The total count of Unicode characters in the first string being compared.

`text2Ptr`  

A pointer to the second Unicode string to compare.

`text2Length`  

The total count of Unicode characters in the second string being compared.

`equivalent`  

A pointer to a `Boolean` value or pass `NULL`. On return, `UCCompareTextDefault` produces a value of `true` if the strings are equivalent for the options you have specified. If you wish simply to sort a list of strings in order, using your specified options, you can pass `NULL` for the `equivalent` parameter and only use the `order` parameter’s result. In this case, all available comparison criteria are used to put the strings in a deterministic order, even if they are considered “equivalent” for the options you have specified. Note that you can set either the `equivalent` or the `order` parameters to `NULL`, but not both.

`order`  

A pointer to a signed, 32-bit integer value, or pass `NULL`. If you wish simply to test the strings for equivalence, using your specified options (which can be much faster than determining ordering), you can pass `NULL` for the `order` parameter and only use the `equivalent` parameter’s result. (Note that either the `equivalent` or the `order` parameters may be `NULL`, but not both.

## Return Value

A result code.

## Discussion

You can call the `UCCompareTextDefault` function when you want to use a simple collation function that requires minimum setup. This function uses the system default collation order (that is, the collation order for a `LocaleRef` of `NULL` and a variant of 0), and it does not require a collator object or collation keys.

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

func UCCompareTextNoLocale(UCCollateOptions, UnsafePointer&lt;UniChar>!, Int, UnsafePointer&lt;UniChar>!, Int, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Int32>!) -> OSStatus

Uses a fixed, locale-insensitive order to compare Unicode strings.

