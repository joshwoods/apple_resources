

- Core Foundation
-  CFStringIsSurrogateHighCharacter(\_:) 

Function

# CFStringIsSurrogateHighCharacter(\_:)

Returns a Boolean value that indicates whether a given character is a high character in a surrogate pair.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringIsSurrogateHighCharacter(_ character: UniChar) -> Bool
```

## Parameters 

`character`  

A UTF-16 character.

## Return Value

`true` if `character` is a high character in a surrogate pair, otherwise `false`.

## See Also

### Managing Surrogates

func CFStringGetLongCharacterForSurrogatePair(UniChar, UniChar) -> UTF32Char

Returns a UTF-32 character that corresponds to a given pair of UTF-16 surrogate characters.

func CFStringGetSurrogatePairForLongCharacter(UTF32Char, UnsafeMutablePointer&lt;UniChar>!) -> Bool

Maps a given UTF-32 character to a pair of UTF-16 surrogate characters.

func CFStringIsSurrogateLowCharacter(UniChar) -> Bool

Returns a Boolean value that indicates whether a given character is a low character in a surrogate pair.

