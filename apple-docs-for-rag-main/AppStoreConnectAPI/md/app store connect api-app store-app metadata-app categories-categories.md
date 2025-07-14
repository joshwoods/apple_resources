

- App Store Connect API
- App Store
- App Metadata
-  App Categories 

API Collection

# App Categories

Get App Store categories and subcategories for apps.

## Overview

`appCategories` provides read-only information that includes the list of choices for an app’s App Store category, subcategory, and secondary category.

To update your app’s categories, use the App Infos resource. For more information about categories, see Choosing a Category.

## Topics

### Listing Categories and Subcategories

List App Categories

List all categories on the App Store, including the category and subcategory hierarchy.

List All Subcategories for an App Category

List all App Store subcategories that belong to a specific category.

### Reading App Category Information

Read App Category Information

Get a specific app category.

Read the Parent Information of an App Category

Get the App Store category to which a specific subcategory belongs.

### Objects

object AppCategoriesResponse

A response that contains a list of App Category resources.

object AppCategory

The data structure that represent an App Categories resource.

object AppCategoryResponse

A response that contains a single App Categories resource.

object AppCategoriesWithoutIncludesResponse

object AppCategoryWithoutIncludesResponse

## See Also

### Managing Categories and Age Declarations

Age Rating Declarations

Update required declarations that determine your app’s age rating.

