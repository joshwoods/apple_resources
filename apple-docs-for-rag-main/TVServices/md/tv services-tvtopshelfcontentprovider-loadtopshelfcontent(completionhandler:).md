

- TV Services
- TVTopShelfContentProvider
-  loadTopShelfContent(completionHandler:) 

Instance Method

# loadTopShelfContent(completionHandler:)

Provides the content you want to display in the top shelf for your app.

tvOS 13.0+

``` source
func loadTopShelfContent(completionHandler: @escaping ((any TVTopShelfContent)?) -> Void)
```

``` source
func loadTopShelfContent() async -> (any TVTopShelfContent)?
```

## Parameters 

`completionHandler`  

The handler block to execute with your content. This block has no return value and takes the following parameter:

content  
The object that describes the content you want to display in the top shelf interface. For example, to display your content in a carousel format, specify a TVTopShelfCarouselContent object with the items you want to display. Specify `nil` if you have no content to display or encounter an error.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func loadTopShelfContent() async -> (any TVTopShelfContent)?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The system calls this method when it needs your app’s top shelf content. In your implementation, create the TVTopShelfItem objects you want to display and wrap them in a matching TVTopShelfContent object. The specific objects you create depends on how you want to display your content. You can display items using one of the following interface styles:

- A *carousel interface* displays TVTopShelfCarouselItem objects in a horizontal line. The user swipes left and right to navigate from item to item.

- A *sectioned interface* groups TVTopShelfSectionedItem objects together and presents them in a scrolling list.

- An *inset interface* organizes either carousel or sectioned items and insets them by a specified amount.

If you call the completionHandler with a `nil` value, the system displays a static image provided by your app.

