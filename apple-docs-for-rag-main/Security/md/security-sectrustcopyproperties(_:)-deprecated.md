

- Security
-  SecTrustCopyProperties(\_:) Deprecated

Function

# SecTrustCopyProperties(\_:)

Returns an array containing the properties of a trust object.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedmacOS 10.7–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecTrustCopyProperties(_ trust: SecTrust) -> CFArray?
```

## Parameters 

`trust`  

The trust object from which properties should be copied.

## Return Value

An array, or `NULL` if the trust object has not yet been evaluated. In Objective-C, call the CFRelease function to free this array’s memory when you are done with it.

## Discussion

The result is an ordered array of dictionaries, one per certificate in the chain, beginning with the leaf node at index zero (`0`) and continuing up to the anchor (or the last certificate in the chain if no anchor was found).

The property dictionary at index zero may also include general information about the entire chain’s validity in the context of this trust evaluation. See Certificate Property Type Values for a list of currently defined keys.

