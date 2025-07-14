

- User Notifications
- UNUserNotificationCenter
-  getNotificationCategories(completionHandler:) 

Instance Method

# getNotificationCategories(completionHandler:)

Fetches your app’s registered notification categories.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
func getNotificationCategories(completionHandler: @escaping (Set) -> Void)
```

``` source
func notificationCategories() async -> Set
```

## Parameters 

`completionHandler`  

The block to execute asynchronously with the results. This block may be executed on a background thread. The block has no return value and takes the following parameter:

categories  
The set of UNNotificationCategory objects containing your registered notification types. If your app has not yet registered any categories, this parameter is an empty set.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func notificationCategories() async -> Set
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to retrieve your app’s currently registered notification types. You might use this method when you want to augment the current set of categories with new categories later on. Simply merge the returned set with any new category objects and register the updated set.

```
let center = UNUserNotificationCenter.current()
let categories = await center.notificationCategories()
```

## See Also

### Managing notification categories

func setNotificationCategories(Set&lt;UNNotificationCategory>)

Registers the notification categories that your app supports.

