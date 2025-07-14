

- Core Foundation
-  CFStringGetLongCharacterForSurrogatePair(\_:\_:) 

Function

# CFStringGetLongCharacterForSurrogatePair(\_:\_:)

Returns a UTF-32 character that corresponds to a given pair of UTF-16 surrogate characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetLongCharacterForSurrogatePair(
    _ surrogateHigh: UniChar,
    _ surrogateLow: UniChar
) -> UTF32Char
```

## Parameters 

`surrogateHigh`  

The high surrogate character.

`surrogateLow`  

The low surrogate character.

## Return Value

A UTF32Char that corresponds to the combination of `surrogateHigh` and `surrogateLow`.

## See Also

### Managing Surrogates

func CFStringGetSurrogatePairForLongCharacter(UTF32Char, UnsafeMutablePointer&lt;UniChar>!) -> Bool

Maps a given UTF-32 character to a pair of UTF-16 surrogate characters.

func CFStringIsSurrogateHighCharacter(UniChar) -> Bool

Returns a Boolean value that indicates whether a given character is a high character in a surrogate pair.

func CFStringIsSurrogateLowCharacter(UniChar) -> Bool

Returns a Boolean value that indicates whether a given character is a low character in a surrogate pair.

