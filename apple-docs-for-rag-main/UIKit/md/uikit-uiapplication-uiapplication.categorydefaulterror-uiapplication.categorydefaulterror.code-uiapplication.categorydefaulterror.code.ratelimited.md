

- UIKit
- UIApplication
- UIApplication.CategoryDefaultError
- UIApplication.CategoryDefaultError.Code
-  UIApplication.CategoryDefaultError.Code.rateLimited 

Case

# UIApplication.CategoryDefaultError.Code.rateLimited

The system didn’t determine if your app is the default in a category because the app made the request too many times.

iOS 18.2+iPadOS 18.2+

``` source
case rateLimited
```

## Discussion

When you receive an error with this code, the error’s user info dictionary contains these keys:

statusLastProvidedDateErrorKey  
The date at which the app most recently received a result indicating whether it’s the default app in a category.

retryAvailableDateErrorKey  
The date at which the app can next request an updated response.

