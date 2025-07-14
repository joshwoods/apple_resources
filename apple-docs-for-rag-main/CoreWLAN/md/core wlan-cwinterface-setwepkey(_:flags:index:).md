

- Core WLAN
- CWInterface
-  setWEPKey(\_:flags:index:) 

Instance Method

# setWEPKey(\_:flags:index:)

Sets the interface WEP key.

macOS 10.6+

``` source
func setWEPKey(
    _ key: Data?,
    flags: CWCipherKeyFlags,
    index: Int
) throws
```

## Parameters 

`key`  

An NSData object containing the WEP key.

`flags`  

An NSUInteger indicating which cipher key flags to use for the specified key.

`index`  

An NSUInteger indicating which default key index to use for the specified key.

## Discussion

*key* must be 5 octets for WEP-40 or 13 octets for WEP-104. If *key* is *nil*, this method clears the WEP key for the interface. *index* must correspond to default key index 1-4.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting interface parameters

func setPairwiseMasterKey(Data?) throws

Sets the interface pairwise primary key (PMK).

func setPower(Bool) throws

Sets the interface power state.

func setWLANChannel(CWChannel) throws

Sets the interface channel.

