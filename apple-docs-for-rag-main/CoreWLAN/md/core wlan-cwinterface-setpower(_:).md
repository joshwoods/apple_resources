

- Core WLAN
- CWInterface
-  setPower(\_:) 

Instance Method

# setPower(\_:)

Sets the interface power state.

macOS 10.6+

``` source
func setPower(_ power: Bool) throws
```

## Parameters 

`power`  

A Boolean value corresponding to the power state. *NO* indicates the “OFF” state.

## Discussion

This operation may require an administrator password.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting interface parameters

func setPairwiseMasterKey(Data?) throws

Sets the interface pairwise primary key (PMK).

func setWEPKey(Data?, flags: CWCipherKeyFlags, index: Int) throws

Sets the interface WEP key.

func setWLANChannel(CWChannel) throws

Sets the interface channel.

