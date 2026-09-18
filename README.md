# Coded UI extension project for WPF TreeGrid

This repository contains a Coded UI extension project for the Syncfusion WPF TreeGrid control. It enables Coded UI tests to recognize and interact with TreeGrid elements such as cells, rows, headers, stacked headers, and row headers in Visual Studio.

## Overview

The project provides custom property providers and wrapper classes for Syncfusion WPF controls so that Coded UI can identify and automate grid elements reliably during UI testing.

## Included components

- `Extensions/` - Coded UI extension logic
- `PropertyProviders/` - custom property providers for grid and header elements
- `WpfControlsClass/` - WPF control wrappers used by Coded UI
- `Properties/` - assembly metadata and generated project resources

## Supported controls

This repository includes support for a range of Syncfusion WPF controls, including:

- SfTreeGrid
- SfTreeGridCell
- SfTreeGridHeaderCell
- SfTreeGridRow
- SfTreeGridRowHeaderCell
- SfTreeGridStackedHeaderCell
- Additional related grid controls such as SfDataGrid, SfGridCell, and header cell wrappers

## Project files

The solution includes Visual Studio project files for multiple versions:

- `Syncfusion.VisualStudio.TestTools.UITest.SfGridExtension.WPF_2010.csproj`
- `Syncfusion.VisualStudio.TestTools.UITest.SfGridExtension.WPF_2012.csproj`
- `Syncfusion.VisualStudio.TestTools.UITest.SfGridExtension.WPF_2013.csproj`
- `Syncfusion.VisualStudio.TestTools.UITest.SfGridExtension.WPF_2015.csproj`

## Requirements

- Visual Studio 2010/2012/2013/2015
- .NET Framework 4.6
- Syncfusion WPF controls (`Syncfusion.SfGrid.WPF` and related assemblies)
- Microsoft Coded UI Test framework

## How to use

1. Open the appropriate solution for your Visual Studio version.
2. Build the project to generate the extension assembly.
3. Reference the built assembly in your Coded UI test project.
4. Use the extended TreeGrid controls in your automated UI tests.

## License

This project is licensed under the MIT License. See the license file for details if available in the repository.

## Reference

This sample is maintained by Syncfusion and demonstrates how to create a Coded UI extension for Syncfusion WPF TreeGrid controls.
