

- UIKit
- UIApplication
-  isDefault(\_:) 

Instance Method

# isDefault(\_:)

Reports whether this app is the person’s default app in the given category.

iOS 18.2+iPadOS 18.2+

``` source
nonisolated
func isDefault(_ category: UIApplication.Category) throws -> Bool
```

## Parameters 

`category`  

The type of app for which you test whether your app is the default.

## Return Value

If the system determines the status of the app, this method returns `true` if the app is the default app in the category, and `false` otherwise. If the system doesn’t determine the status, or the app exceeds the threshold rate for calling this method, it throws an error.

## Discussion

To reduce the likelihood that users face continuous requests to set a browser as their default, this API only tells the browser app if it’s the default up to four times in a year. If you call the method too frequently, it throws an error with the domain UIApplicationCategoryDefaultErrorDomain and the code rateLimited. The error’s user information dictionary contains these keys:

statusLastProvidedDateErrorKey  
The date at which the app most recently received a `true` or `false` response from this method.

retryAvailableDateErrorKey  
The date at which the app can next request an updated response.

## See Also

### Discovering if your app is the default app in a category

enum Category

Constants that describe the types of apps in the system.

struct CategoryDefaultError

Errors that can happen when the system checks if your app is the default app in a category.

