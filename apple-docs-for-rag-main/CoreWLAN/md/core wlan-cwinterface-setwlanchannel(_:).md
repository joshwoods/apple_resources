

- Core WLAN
- CWInterface
-  setWLANChannel(\_:) 

Instance Method

# setWLANChannel(\_:)

Sets the interface channel.

macOS 10.7+

``` source
func setWLANChannel(_ channel: CWChannel) throws
```

## Parameters 

`channel`  

A CWChannel object corresponding to the channel.

## Discussion

The channel cannot be changed if the interface is associated to a network.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting interface parameters

func setPairwiseMasterKey(Data?) throws

Sets the interface pairwise primary key (PMK).

func setPower(Bool) throws

Sets the interface power state.

func setWEPKey(Data?, flags: CWCipherKeyFlags, index: Int) throws

Sets the interface WEP key.

