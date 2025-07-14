

- Notification Center
- NCWidgetProviding
-  widgetPerformUpdate(completionHandler:) Deprecated

Instance Method

# widgetPerformUpdate(completionHandler:)

Called to give a widget an opportunity to update its contents.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 8.0–14.0DeprecatedmacOS 10.10–11.0Deprecated

``` source
optional func widgetPerformUpdate(completionHandler: @escaping (NCUpdateResult) -> Void)
```

``` source
optional func widgetPerformUpdate() async -> NCUpdateResult
```

Deprecated

Use WidgetKit instead.

## Parameters 

`completionHandler`  

A block to be called when the widget’s content has been updated.

The block takes the following parameter:

result  
A value of type `NCUpdateResult` that describes the result of the update procedure. (NCUpdateResult lists the possible values of `result`.)

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method is called to give a widget an opportunity to update its contents and redraw its view prior to an operation such as a snapshot. When the widget is finished updating its contents (and redrawing, if necessary), the widget should call the completion handler block, passing the appropriate `NCUpdateResult` value.

## See Also

### Updating a Widget’s Contents

enum NCUpdateResult

The result of updating a widget’s state.

Deprecated

