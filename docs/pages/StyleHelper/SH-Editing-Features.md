---
layout: default
title: Editing Features
parent: Style Helper User Guide
nav_order: 3
---

# Editing Features
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

# Editing Features

Style Helper provides comprehensive editing capabilities for customizing table data, editing style data properties, and performing batch operations for efficient data edition.

## Overview

The editing features include:
- **Table Column Preferences** - Configure table structure and data display.
- **Data Editing** - Edit style properties for all three tabs.
- **Batch Editing** - Edit multiple objects and rows simultaneously.
- **Find and Replace** - Find and replace property values quickly across selected columns.
- **Children Styles Support** - Edit children nested label styles.


## Table Customization

### Customizing Table Data Structure

Style Helper allows you to customize the table structure to show only the data you need:

#### Preferences Button
- **Independent Control** - Each tab has its own Preferences button for column configuration.
- **Dynamic Configuration** - Available column options change based on checked objects.
- **Tab-Specific Settings** - Column settings are configured independently for each tab.

#### Column Preferences
After accessing the preferences, you can:
- **Add Columns** - By adding new properties adds new columns.
- **Remove Columns** - Remove unnecessary columns.
- **Reorder Columns** - Arrange columns in preferred order.


![Table customization and profile management](../../../assets/images/GIFs/SH/Table-customization-and-profile-management.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

## Data Editing for the Different Tabs

### Styles Tab Editing

Edit Civil 3D object style property data directly in the table:

#### Editing Property Data Process

1. **Access the Tab** - Open the Styles tab you want to edit.
2. **Check Objects** - Check specific objects to work with.
3. **Configure Columns** - Use Preferences button to configure table columns.
4. **Edit Properties** - Modify style properties directly in the table.
5. **Save Changes** - Changes are applied.

![Object Styles tab editing process](../../../assets/images/GIFs/SH/Object-Styles-tab-editing-process.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

![Label Styles tab editing process](../../../assets/images/GIFs/SH/Label-Styles-tab-editing-process.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

![Table Styles tab editing process](../../../assets/images/GIFs/SH/Table-Styles-tab-editing-process.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

## Batch Editing

### Multiple Row Data Editing

Edit multiple objects, style or table rows simultaneously for efficient workflow:

#### Selection Process
- **Multi-selection** - Select multiple rows in the table.
- **Bulk Modifications** - Apply changes to one column object and the change will be propagated to the set of selected rows at once.
- **Efficiency** - Save time with bulk operations.
- **Visual Validation** - See which objects or rows are affected by changes based on the status column.
- **Apply Changes** - Apply changes to the modified items.

![Multi-row editing process](../../../assets/images/GIFs/SH/Multi-row-editing-process.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

### Main Component–Subcomponent Relationships in Batch Editing

Since the tool displays all subcomponents, some data may be associated with the main component. Editing a property of the main component can affect multiple rows, because the main component controls several subcomponents.

#### Understanding Main Component–Subcomponent Data
- **Main Component Properties** – Some data belongs to the main component.
- **Subcomponents** – Subcomponents have their own specific data.
- **Multiple Row Impact** – Editing main component properties can impact multiple rows.

#### Main Component Property Editing
- **Main Component Changes** – Changes to main component properties affect all related subcomponents.
- **Cascading Updates** – Updates to the main component automatically update its subcomponents.
- **Bulk Modifications** – Modify main component properties to update several subcomponents at once.

> **Note:** To identify which rows represent subcomponents or main components during batch editing, refer to the **Component** column in the table. The structure and naming in the Component column are explained in the following reference: [Component Column Reference](SH-Object-Label-Table-Styles.md#component-column-reference)

<!-- ![Parent-child relationship editing and its impact on multiple rows](../../../assets/images/GIFs/SH/Parent-child-relationship-editing-and-its-impact-on-multiple-rows.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub> -->

## Find and Replace

The Find and Replace feature allows you to quickly find current editable property values and replace them across multiple columns, making bulk editing operations more efficient.

### Overview

Style Helper provides a find and replace functionality that enables you to:
- Find specific text values in selected columns
- Replace found values with new text
- Add prefixes and suffixes to values
- Apply changes only to selected rows (optional)
- Work with multiple columns simultaneously

### How It Works

The Style Helper feature includes the following options:


#### Find on Columns
- **Multiselection Dropdown** - Select the columns where you want to search for values. You can select multiple columns to perform the find and replace operation.

#### Find and Replace Inputs
- **Find** - Enter the text value you want to find in the selected columns.
- **Replace** - Enter the new text value that will replace the found text.
- **Prefix** - Optional text to add at the beginning of the replaced value.
- **Suffix** - Optional text to add at the end of the replaced value.

**Example:**
- Current Text value: `ABC_TextToFind_1`
- Find: `TextToFind`
- Replace: `ReplacedText`
- Prefix: `Prefix-`
- Suffix: `-Sufix`
- Edited text value: `Prefix-ABC_ReplacedText_1-Sufix`

#### Find Only on Selected Rows
- **Boolean Option** - When enabled, the find and replace operation applies only to currently selected rows in the table. When disabled, the operation applies to all rows in the table.


### Usage

1. **Select Rows (Optional)** - If you want to limit the operation to specific rows, select them in the table first.
2. **Enable Find Only on Selected Rows(Optional)** - Check this option if you want to restrict the operation to selected rows only.
3. **Select Columns** - Use the "Find on Columns" multiselection dropdown to choose one or more columns where you want to search.
4. **Enter Find Value** - Type the text you want to find in the Find field.
5. **Enter Replace Value** - Type the replacement text in the Replace field.
6. **Add Prefix/Suffix (Optional)** - If needed, enter prefix and/or suffix values.
7. **Apply Changes** - The values are edited in the main UI and marked as edited status. Values are applied when you apply changes in the main UI.

**Important Notes:**

- Values are applied only when the user applies changes in the main UI.
- The operation works with editable properties only.

![Style Helper find and replace feature](../../../assets/images/GIFs/SH/SH-Style-Helper-Find-Replace.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub>

## Missing Object Limitations

Due to current Civil 3D API limitations, Style Helper cannot collect the following style types:

- **Section View Styles** - Drafting buffer outline.
- **Rail Turnout** - All rail turnout related styles.
- **Can't View Styles** - Equilibrium can't line annotation, Applied can't line annotation.
- **Bridge Styles** - All bridge related styles.

These limitations are imposed by the Civil 3D API and are not within the control of Style Helper. We continue to monitor API updates and will add support for these styles when they become available through the Civil 3D API.


## Label Styles Children Component Editing

Style Helper supports children label styles editing capabilities.

Civil 3D has hierarchical component structures for label styles:

- **Parent label Styles** - Main style objects (e.g., Point Label Styles)
- **Child Label Style** - Inside the parent label style it could have additional nested children and subchildren label styles. We are also supporting these.


<!-- ![Overview of editing features](../../../assets/images/GIFs/SH/Overview-of-editing-features.gif)
<sub>Note: the version on the image may not reflect the [latest version of DiCivil Package](https://diroots.com/civil3D-plugins/DiCivil/).</sub> -->