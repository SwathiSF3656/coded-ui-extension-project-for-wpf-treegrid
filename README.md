# Coded UI Extension Project for WPF Tree Grid

This repository contains a Coded UI Test extension for the Syncfusion WPF Tree Grid control. The project provides custom property providers and wrapper classes that allow Visual Studio Coded UI Test to recognize and interact with grid elements more effectively during automated UI testing.

## Overview

The extension includes:

- Custom property support for Syncfusion WPF Tree Grid controls
- UI wrapper classes for WPF Tree Grid elements
- Property providers for rows, cells, headers, and grouped content
- Visual Studio extension registration for Coded UI test automation

This makes it easier to write robust UI automation tests for applications that use Syncfusion's WPF Tree Grid control.

## Supported capabilities

The extension exposes custom WPF Tree Grid properties such as:

- RowCount
- ColumnCount
- SelectionMode
- SelectedIndex
- SelectedItemCount

It also provides support for related WPF Tree Grid elements like:

- WPF Tree Grid rows
- WPF Tree Grid cells
- Header cells
- Row header cells
- Stacked header cells
- Details view data grid
- Group drop area items

## Project structure

- `Extensions/` - Visual Studio extension registration and package setup
- `PropertyProviders/` - UI property providers for WPF Tree Grid and related controls
- `WpfControlsClass/` - WPF wrapper classes used by Coded UI tests
- `Properties/` - Assembly metadata and resource information
- `*.sln` files - Solutions for Visual Studio 2010, 2012, 2013, and 2015
- `*.csproj` files - Project files for the corresponding Visual Studio versions

## Build requirements

- Microsoft Visual Studio 2010, 2012, 2013, or 2015
- .NET Framework 4.6
- Syncfusion WPF controls (WPF Tree Grid, WPF Data Grid, and related assemblies)
- Visual Studio Coded UI Test / UI automation support

## How to use

1. Open the appropriate solution file based on your Visual Studio version.
2. Restore the required Syncfusion assemblies.
3. Build the project.
4. Reference the generated assembly in your Coded UI Test project.
5. Use the provided `WpfSfTreeGrid` and related wrappers to locate and validate WPF Tree Grid elements in automated tests.

## Example

```csharp
var treeGrid = new WpfSfTreeGrid();
treeGrid.SearchProperties[UITestControl.PropertyNames.Name] = "sfTreeGrid";

int rowCount = (int)treeGrid.GetProperty(WpfSfTreeGrid.PropertyNames.RowCount);
int selectedIndex = (int)treeGrid.GetProperty(WpfSfTreeGrid.PropertyNames.SelectedIndex);
