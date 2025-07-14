

- CKTool JS
- CancellablePromise
-  then 

Instance Method

# then

Tells `CancellablePromise` what callbacks to call on success or failure of the inner promise.

CKTool JS 1.2.15+

``` source
CancellablePromise then(
 Function? onrejected,
 Function? onfullfilled
);
```

## Parameters 

`onrejected`  

An optional function `CancellablePromise` calls when the inner promise rejects.

`onfullfilled`  

An optional function `CancellablePromise` calls when the inner promise resolves successfully.

## Discussion

If you provide a function for the `onrejected` parameter, `CancellablePromise` will call that function if the promise fails.

If you provide a function for the `onfulfilled` parameter, `CancellablePromise` will call that function if the promise succeeds.

