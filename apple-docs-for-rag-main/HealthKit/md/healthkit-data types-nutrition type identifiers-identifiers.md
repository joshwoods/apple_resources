

- HealthKit
- Data types
-  Nutrition Type Identifiers 

API Collection

# Nutrition Type Identifiers

Type identifiers used for tracking diet and nutrition.

## Overview

Nutritional data can be broadly categorized into two main groups:

- Macronutrients consumed in large quantities, such as fats, carbohydrates, and proteins.

- Micronutrients consumed in smaller quantities, such as vitamins and minerals.

HealthKit also provides type identifiers for nutrition-related items that users may want to track, like water or caffeine.

You do not need to track all nutritional information; you can focus on the items of interest to your users. In general, the data from nutrition labels is a good place to start. Many countries and regions require a nutrition label on packaged food. While the contents of these labels vary from one country or region to another, they typically include the nutritional data represented by these properties:

- dietaryEnergyConsumed

- dietaryFatTotal

- dietaryFatSaturated

- dietaryCholesterol

- dietaryCarbohydrates

- dietaryFiber

- dietarySugar

- dietaryProtein

- dietaryCalcium

- dietaryIron

- dietaryPotassium

- dietarySodium

- dietaryVitaminA

- dietaryVitaminC

- dietaryVitaminD

### Combine Nutritional Samples

Macronutrient identifiers can be thought of as a hierarchy. The dietaryEnergyConsumed identifier represents the total amount of energy from all fats, carbohydrates, and protein. You can provide a detailed breakdown using the dietaryFatTotal, dietaryCarbohydrates, and dietaryProtein identifiers. Fats can be further separated into dietaryFatMonounsaturated, dietaryFatPolyunsaturated, and dietaryFatSaturated. Carbohydrates can be identified as dietaryFiber and dietarySugar.

Unless your app is very focused (for example, tracking only sugar or saturated fat), always provide the total data (dietaryFatTotal or dietaryCarbohydrates), and then optionally provide the more detailed information using the subcategories. You do not need to provide data for all of the subcategories; however, the sum of the subcategory sample values should be equal or less than the total sample’s value.

Note

The dietaryEnergyConsumed samples are handled differently than the other macronutrients. While it can be seen as a total value, dietaryEnergyConsumed is measured in calories or kilojoules, while the individual macronutrient samples are measured by mass.

## Topics

### Essentials

static let food: HKCorrelationTypeIdentifier

Food correlation types combine any number of nutritional samples into a single food object.

let HKMetadataKeyFoodType: String

The type of food that the HealthKit object represents.

### Macronutrients

static let dietaryEnergyConsumed: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of energy consumed.

static let dietaryCarbohydrates: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of carbohydrates consumed.

static let dietaryFiber: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of fiber consumed.

static let dietarySugar: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of sugar consumed.

static let dietaryFatTotal: HKQuantityTypeIdentifier

A quantity sample type that measures the total amount of fat consumed.

static let dietaryFatMonounsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of monounsaturated fat consumed.

static let dietaryFatPolyunsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of polyunsaturated fat consumed.

static let dietaryFatSaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of saturated fat consumed.

static let dietaryCholesterol: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of cholesterol consumed.

static let dietaryProtein: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of protein consumed.

### Vitamins

static let dietaryVitaminA: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin A consumed.

static let dietaryThiamin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of thiamin (vitamin B1) consumed.

static let dietaryRiboflavin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of riboflavin (vitamin B2) consumed.

static let dietaryNiacin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of niacin (vitamin B3) consumed.

static let dietaryPantothenicAcid: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of pantothenic acid (vitamin B5) consumed.

static let dietaryVitaminB6: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of pyridoxine (vitamin B6) consumed.

static let dietaryBiotin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of biotin (vitamin B7) consumed.

static let dietaryVitaminB12: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of cyanocobalamin (vitamin B12) consumed.

static let dietaryVitaminC: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin C consumed.

static let dietaryVitaminD: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin D consumed.

static let dietaryVitaminE: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin E consumed.

static let dietaryVitaminK: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin K consumed.

static let dietaryFolate: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of folate (folic acid) consumed.

### Minerals

static let dietaryCalcium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of calcium consumed.

static let dietaryChloride: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of chloride consumed.

static let dietaryIron: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of iron consumed.

static let dietaryMagnesium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of magnesium consumed.

static let dietaryPhosphorus: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of phosphorus consumed.

static let dietaryPotassium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of potassium consumed.

static let dietarySodium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of sodium consumed.

static let dietaryZinc: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of zinc consumed.

### Hydration

static let dietaryWater: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of water consumed.

### Caffeination

static let dietaryCaffeine: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of caffeine consumed.

### Ultratrace Minerals

static let dietaryChromium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of chromium consumed.

static let dietaryCopper: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of copper consumed.

static let dietaryIodine: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of iodine consumed.

static let dietaryManganese: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of manganese consumed.

static let dietaryMolybdenum: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of molybdenum consumed.

static let dietarySelenium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of selenium consumed.

