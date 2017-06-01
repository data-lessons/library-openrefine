---
title: "Basic OpenRefine functions I: Layout, Organizing Columns, and Sorting"
teaching: 5
exercises: 10
questions:
- "How do I move, rename or remove columns in OpenRefine?"
- "How do I sort data in OpenRefine?"
objectives:
- "Explain how to reorder, rename and remove columns"
- "Explain how to sort data in columns"

keypoints:
- "You can reorder, rename and remove columns in OpenRefine"
---

## The layout of OpenRefine

For this lesson, I'm going to demonstrate some of the features of OpenRefine with the dataset 'UCSDGuardian.csv' You can either simply pay attention as I work through the demo, or you may open the UCSDGuardian file as a new project and follow along. The exercise that follows the short demo will use the 'doaj-article-sample.csv' file you just used to create a project.

OpenRefine displays data in a tabular format. Each row will usually represent a 'record' in the data, while each column represents a type of information. This is very similar to how you might view data in a spreadsheet or database. If you look at the top left of the data sheet, under the solid blue header, you'll see an option to change to the record view. In this case, it doesn't really change anything since we have records of one level, so to speak. If you are importing an xml or DDI file that has a hierarchical structure, the data view will look different, showing the structure of the record.

OpenRefine only displays a limited number of lines of data at one time. You can adjust the number choosing between 5, 10 (the default), 25 and 50.

## Reordering and renaming columns
Many operations in OpenRefine are accessed from the drop down menus at the top of each column. You can re-order the columns by clicking the drop down menu at the top of the first column (labelled 'All'), and choosing 'Edit columns->Re-order / remove columns …'

You can then drag and drop column names to re-order the columns, or remove columns completely if they are not required.

> Click on 'All', 'Edit columns->Re-order / remove'. Move Language to just before Translation. Remove Varients 11 - 16.


## Sorting data
You can sort data in OpenRefine by clicking on the drop down menu for the column you want to sort on, and choosing 'Sort'

A box will appear, giving you sort options.

> Go to the Note:Series column, click Sort. 

You can sort by cell value (data, text), by ascending/descending and by type of cell value, meaning valid values, errors or blanks. These options can be very useful for data analysis and cleanup. For now, let's just sort by text and leave the rest of the defaults as they are.

> Click on OK.

Once you have sorted the data a new 'Sort' drop down menu will be displayed.

> Go back to the Note:Series column and click on sort again.

Unlike Excel 'Sorts' in OpenRefine are temporary - that is, if you remove the 'Sort', the data will go back to it's original 'unordered' state. The 'Sort' drop down menu lets you amend the existing sort (e.g. reverse the sort order), remove existing sorts, and make sorts permanent.

> Click on Sort Reverse. 

Sort reverse has changed the sort from Ascending to Descending.

> Click on Sort. In Sort window move Blanks to the first position and click OK.

There are records in my data that have the series note blank. This is something I would want to look into.

You can sort on multiple columns at the same time by adding another sorted column (in the same way).

To rename a column, click on the arrow at the top of the column, then to Edit Column, and then to Rename this Column.

## Exercise Two

1. Re-open or Create your doaj-article-sample project.

2. Sort on the License column. 
	* Is there more than one type of license for this dataset?
	* Are there any records that don't have a license?
	* The date field header doesn't indicate what the date means.  Use Sort to evaluate the date field. What can you conclude about the contents of the date field by using Sort?
	* Rename the date column to indicate what kind of date you think it is.
