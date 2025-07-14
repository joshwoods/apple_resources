

- CKTool JS
- CancellablePromise
-  catch 

Instance Method

# catch

Tells `CancellablePromise` what callback to call on failure of the inner promise.

CKTool JS 1.2.15+

``` source
CancellablePromise catch(
 Function? onrejected
);
```

## Parameters 

`onrejected`  

An optional function `CancellablePromise` calls when the inner promise rejects.

## Discussion

If you provide a function for the `onrejected` parameter, `CancellablePromise` calls that function if the promise fails.

