

- Create ML
- MLDataTable
-  Data Table Derivation Operations 

API Collection

# Data Table Derivation Operations

Create new data tables by manipulating an existing data table.

## Overview

Use these methods to preprocess your data programmatically in Create ML before training a model. For example, you can create a data table by merging two data tables, fill in missing values, and then discarding duplicate rows.

All of these methods create new data tables, leaving the original data table unmodified.

## Topics

### Aggregating Rows

func group&lt;S>(columnsNamed: String..., aggregators: S) -> MLDataTable

Creates a new data table with the given columns and adds a new column for each of the given aggregators.

struct Aggregator

A collection of column operations you can use with a data table’s `group` method.

### Sorting Rows

func sort(columnNamed: String, byIncreasingOrder: Bool) -> MLDataTable

Creates a new data table by sorting the table by the given column.

### Splitting a Data Table

func randomSplit(by: Double, seed: Int) -> (MLDataTable, MLDataTable)

Creates two mutually exclusive, randomly divided subsets of the table.

### Merging Data Tables

func join(with: MLDataTable, on: String..., type: MLDataTable.JoinType) -> MLDataTable

Creates a new data table by merging two data tables by the given columns.

enum JoinType

Join types available for MLDataTable join operations.

### Filling in Missing Values

func fillMissing(columnNamed: String, with: MLDataValue) -> MLDataTable

Creates a modified copy of the table by filling in the missing values in the named column.

### Masking Rows

subscript(MLDataColumn&lt;Bool>) -> MLDataTable

Creates a subset of the table by masking the rows with the given column of Booleans.

subscript(MLUntypedColumn) -> MLDataTable

Creates a subset of the table by masking the rows with the given untyped column.

### Discarding Rows

func dropMissing() -> MLDataTable

Creates a subset of the table by removing any row missing one or more values.

func dropDuplicates() -> MLDataTable

Creates a subset of the table by removing all duplicate rows.

func exclude&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by excluding the rows that contain any of the given values in the given column.

func randomSample(by: Double, seed: Int) -> MLDataTable

Creates a subset of the table by randomly selecting the given proportion of rows.

### Selecting Rows

subscript(Range&lt;Int>) -> MLDataTable

Creates a subset of the table given a range of rows.

subscript&lt;R>(R) -> MLDataTable

Creates a subset of the table given a range expression of rows.

func prefix(Int) -> MLDataTable

Creates a subset of the table given a number of initial rows.

func suffix(Int) -> MLDataTable

Creates a subset of the table given a number of final rows.

func intersect&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by including the rows that contain any of the given values in the given column.

### Selecting Columns

subscript&lt;S>(S) -> MLDataTable

Creates a subset of the table given a sequence of column names.

### Compacting Rows

func condense(columnNamed: String, to: String) -> MLDataTable

Creates a new data table where duplicate row values in the given column are condensed into a new sequence-type column.

### Expanding Rows

func expand(columnNamed: String, to: String) -> MLDataTable

Creates a new data table where duplicate row values in the given column are condensed into a new sequence-type column.

### Compacting Columns

func pack(columnsNamed: String..., to: String, type: MLDataTable.PackType, filling: MLDataValue) -> MLDataTable

Creates a new data table with an additional column that contains the combined values of the given columns.

enum PackType

The storage operations for combining multiple columns into one.

### Expanding Columns

func unpack(columnNamed: String, valueTypes: [MLDataValue.ValueType]?, indexSubset: [Int]?, keySubset: [String]?) -> MLDataTable

Creates a new data table with additional columns that contain the unpacked collections in the given column.

