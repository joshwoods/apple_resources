

- File Provider
- NSFileProviderReplicatedExtension
-  importDidFinish(completionHandler:) 

Instance Method

# importDidFinish(completionHandler:)

Tells the File Provider extension that the system finished importing items.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional func importDidFinish(completionHandler: @escaping () -> Void)
```

``` source
optional func importDidFinish() async
```

## Parameters 

`completionHandler`  

A block that your implementation must call.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func importDidFinish() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The system calls this method after importing on-disk items. You can trigger an import by calling either reimportItems(below:completionHandler:) or import(_:fromDirectoryAt:completionHandler:). The system can also initiate its own imports as needed.

During the import, the system calls your File Provider extension’s createItem(basedOn:fields:contents:options:request:completionHandler:) method and passes the mayAlreadyExist option. Check to see if the item already exists in your remote storage—uploading it if necessary.

After importing all the items, the system calls your importDidFinish(completionHandler:) method. Handle any necessary cleanup operations, and then call the completion handler.

