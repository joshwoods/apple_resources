

- CKTool JS
- CancellablePromise
-  finally 

Instance Method

# finally

Tells `CancellablePromise` what callback to call when the inner promise either succeeds or fails.

CKTool JS 1.2.15+

``` source
CancellablePromise finally(
 Function? onfinally
);
```

## Parameters 

`onfinally`  

An optional function `CancellablePromise` calls when the inner promise succeeds or fails.

## Discussion

If you provide a function for the `onfinally` parameter, `CancellablePromise` calls that function after the promise succeeds or fails.

