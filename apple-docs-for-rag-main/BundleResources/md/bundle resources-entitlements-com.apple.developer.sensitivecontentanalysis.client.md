

- Bundle Resources
- Entitlements
-  com.apple.developer.sensitivecontentanalysis.client 

Property List Key

# com.apple.developer.sensitivecontentanalysis.client

A code-signing entitlement that enables an app to detect nudity in images and video.

iOS 17.0+iPadOS 17.0+

## Details 

Type  

array of strings

## Possible Values 

`analysis`  

## Discussion

The SensitiveContentAnalysis framework fails to return positive results for apps that lack this entitlement in its code signature.

You can add this entitlement to your app by enabling the Sensitive Content Analysis capability in Xcode. For more information, see Detecting nudity in media and providing intervention options.

