---
title: "Basic OpenRefine Functions: Working with columns and using the sort function"
teaching: 10
exercises: 15
questions:
- "How do I move, rename or remove columns in OpenRefine?"
- "How do I sort data in OpenRefine?"
objectives:
- "Explain how to reorder, rename and remove columns"
- "Explain how to sort data in columns"
keypoints:
- "You can reorder, rename and remove columns in OpenRefine"
- "You can use the sort function to find blanks, errors, or evaluate the data in a column"

---

## The layout of OpenRefine
OpenRefine displays data in a tabular format. Each row will usually represent a 'record' in the data, while each column represents a type of information. This is very similar to how you might view data in a spreadsheet or database.

OpenRefine only displays a limited number of lines of data at one time. You can adjust the number choosing between 5, 10 (the default), 25 and 50.

## Reordering and renaming columns
Many operations in OpenRefine are accessed from the drop down menus at the top of each column. You can re-order the columns by clicking the drop down menu at the top of the first column (labelled 'All'), and choosing 'Edit columns->Re-order / remove columns …'

You can then drag and drop column names to re-order the columns, or remove columns completely if they are not required.

## Sorting data
You can sort data in OpenRefine by clicking on the drop down menu for the column you want to sort on, and choosing 'Sort'. Note that in the 'Sort' pop-up box, on the right is an option to find blanks or errors.

Once you have sorted the data a new 'Sort' drop down menu will be displayed.

Unlike Excel 'Sorts' in OpenRefine are temporary - that is, if you remove the 'Sort', the data will go back to it's original 'unordered' state. The 'Sort' drop down menu lets you amend the existing sort (e.g. reverse the sort order), remove existing sorts, and make sorts permanent.

You can sort on multiple columns at the same time by adding another sorted column (in the same way).

Exercise

>## Open a project in OpenRefine
>Open the 'UCSD_Guardian.csv' project in OpenRefine.
>
>>## Solution
>>* Run OpenRefine
>>* Click '<<Open Project >>' and select the 'UCSD_Guardian.csv' file (or, if you haven't yet created the project, do so now).
>>* You should end with the UCSD_Guardian.csv' data visible in OpenRefine. Note that Open Refine saves your changes as you work, so that if you had made changes and then closed OpenRefine, those changes will be there when re-oened.

>## Reorder and delete columns in OpenRefine
>Delete the columns 'File Use' and 'Level'.  Move 'Note:publication' and 'Note:publication2' between the columns 'Variant16' and 'Begin date'
>
>>## Solution
>>* Click on the drop-down arrow at the top of the first column.
>>* Edit columns->Re-order / remove columns …'
>>* In the pop-up box that appears, drag the columns to delete into the right-hand box. Drag and drop in the left-hand box to reorder columns.

>## Sort data in OpenRefine.
>Sort the column 'Note:series' in ascending order, and change the 'Show' setting to 50 rows. 
>
>>## Solution
>>* Click on the drop-down arrow at the top of the 'Note:series' column and choose 'Sort'.
>>* In the pop-up window, make sure the setting is on 'text' and 'a-z' and click 'OK'. The first record's data should be 'Volume 1, Issue 1'.
>>* On the left of the data sheet, directly below the blue header bar, click on '50' in the "Show: 5 10 25 50 rows' option.
>
>## Evaluate the results of the sort: is this an efficient way to discover whether UCSD is missing issues from the Guardian? Are there any records with no assigned Volume/Issue data? After your evaluation, remove the sort.
>
>>## Solution
>>* No, it is not efficient. This data is text, and the 'text' sort sorts one digit at a time instead of an entire number, so that issue 100 comes before issue 2.
>>* At the top of the 'Note:series' column, lick on 'Sort' and in right-hand pane of the pop-up window, drag 'Blanks' to the top and click OK. You will see that there are records with blank values in the 'Note:series' field.
>>*Click on 'Sort' and scroll to 'Remove sort'