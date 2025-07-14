

- Bundle Resources
- Information Property List
-  NSPhotoLibraryUsageDescription 

Property List Key

# NSPhotoLibraryUsageDescription

A message that tells the user why the app is requesting access to the user’s photo library.

iOS 6.0+iPadOS 6.0+macOS 10.14+visionOS 1.0+

## Details 

Name  
Privacy - Photo Library Usage Description

Type  

string

## Mentioned in 

Requesting Authorization for Media Capture on macOS

## Discussion

If your app only adds assets to the photo library and does not read assets, use the NSPhotoLibraryAddUsageDescription key instead.

Important

This key is required if your app uses APIs that have read or write access to the user’s photo library.

## See Also

### Photos

Delivering an Enhanced Privacy Experience in Your Photos App

Adopt the latest privacy enhancements to deliver advanced user-privacy controls.

NSPhotoLibraryAddUsageDescription

A message that tells the user why the app is requesting add-only access to the user’s photo library.

**Name:** Privacy - Photo Library Additions Usage Description

