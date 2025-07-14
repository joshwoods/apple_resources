

- FamilyControls
-  FamilyActivityIconView 

Structure

# FamilyActivityIconView

A type-erased view representing the icon of the family activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor @preconcurrency
struct FamilyActivityIconView
```

## Overview

Family Controls uses this type as a generic constraint for the `Icon` of the Label instances it creates.

## Topics

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Label Constraints

struct FamilyActivityTitleView

A type-erased view representing the title of the family activity.

