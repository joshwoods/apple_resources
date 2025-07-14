

- Core WLAN
- CWInterface
-  setPairwiseMasterKey(\_:) 

Instance Method

# setPairwiseMasterKey(\_:)

Sets the interface pairwise primary key (PMK).

macOS 10.6+

``` source
func setPairwiseMasterKey(_ key: Data?) throws
```

## Parameters 

`key`  

An NSData object containing the pairwise primary key (PMK).

## Discussion

*key* must be 32 octets. If *key* is *nil*, this method clears the PMK for the interface.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting interface parameters

func setPower(Bool) throws

Sets the interface power state.

func setWEPKey(Data?, flags: CWCipherKeyFlags, index: Int) throws

Sets the interface WEP key.

func setWLANChannel(CWChannel) throws

Sets the interface channel.

