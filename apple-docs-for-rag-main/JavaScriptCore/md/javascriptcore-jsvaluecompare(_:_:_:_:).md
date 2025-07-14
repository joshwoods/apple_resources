

- JavaScriptCore
-  JSValueCompare(\_:\_:\_:\_:) 

Function

# JSValueCompare(\_:\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 9.0+visionOS 2.0+

``` source
func JSValueCompare(
    _ ctx: JSContextRef,
    _ left: JSValueRef,
    _ right: JSValueRef,
    _ exception: UnsafeMutablePointer?
) -> JSRelationCondition
```

## Discussion

```
@function
@abstract         Compares two JSValues.
@param ctx        The execution context to use.
@param left       The JSValue as the left operand.
@param right      The JSValue as the right operand.
@param exception  A pointer to a JSValueRef in which to store an exception, if any. To reliable detect exception, initialize this to null before the call. Pass NULL if you do not care to store an exception.
@result           A value of JSRelationCondition, a kJSRelationConditionUndefined is returned if an exception is thrown.
@discussion       The result is computed by comparing the results of JavaScript's `==`, `` operators. If either `left` or `right` is (or would coerce to) `NaN` in JavaScript, then the result is kJSRelationConditionUndefined.
```

