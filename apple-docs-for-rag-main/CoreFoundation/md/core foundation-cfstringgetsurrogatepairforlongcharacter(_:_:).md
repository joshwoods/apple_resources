

- Core Foundation
-  CFStringGetSurrogatePairForLongCharacter(\_:\_:) 

Function

# CFStringGetSurrogatePairForLongCharacter(\_:\_:)

Maps a given UTF-32 character to a pair of UTF-16 surrogate characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetSurrogatePairForLongCharacter(
    _ character: UTF32Char,
    _ surrogates: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`character`  

A UTF-32 character.

`surrogates`  

A buffer to contain the returned surrogate pair.

The buffer must have space for at least 2 UTF-16 characters.

## Return Value

`true` if `character` is mapped to a surrogate pair, otherwise `false`.

## See Also

### Managing Surrogates

func CFStringGetLongCharacterForSurrogatePair(UniChar, UniChar) -> UTF32Char

Returns a UTF-32 character that corresponds to a given pair of UTF-16 surrogate characters.

func CFStringIsSurrogateHighCharacter(UniChar) -> Bool

Returns a Boolean value that indicates whether a given character is a high character in a surrogate pair.

func CFStringIsSurrogateLowCharacter(UniChar) -> Bool

Returns a Boolean value that indicates whether a given character is a low character in a surrogate pair.

