

- Create ML
-  Data Visualizations 

API Collection

# Data Visualizations

Render images of data tables and columns in a playground.

## Topics

### Table Visualizations

func show(MLDataTable) -> any MLStreamingVisualizable

Generates a streaming visualization of the data table.

Deprecated

### Column Visualizations

func show&lt;Element>(MLDataColumn&lt;Element>) -> any MLStreamingVisualizable

Generates a streaming visualization of the data column.

Deprecated

func show(MLUntypedColumn) -> any MLStreamingVisualizable

Generates a streaming visualization of the untyped column.

Deprecated

### Plot Visualizations

func show&lt;ElementX, ElementY>(MLDataColumn&lt;ElementX>, MLDataColumn&lt;ElementY>) -> any MLStreamingVisualizable

Generates a streaming plot visualization of the two data columns.

Deprecated

func show(MLUntypedColumn, MLUntypedColumn) -> any MLStreamingVisualizable

Generates a streaming plot visualization of the two untyped columns.

Deprecated

### Visualization Protocols

protocol MLVisualizable

An image visualization of machine learning types.

protocol MLStreamingVisualizable

A sequence of image visualizations for machine learning types.

## See Also

### Tabular Data

struct MLDataTable

A table of data for training or evaluating a machine learning model.

enum MLDataValue

The value of a cell in a data table.

