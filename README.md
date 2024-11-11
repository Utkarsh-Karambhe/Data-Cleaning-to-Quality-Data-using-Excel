# Data-Cleaning-to-Quality-Data-using-Excel
This document provides a step-by-step guide to optimize data readability and formatting in Excel. It covers tasks like adjusting column widths, removing duplicates, trimming spaces, and standardizing text formats, helping to enhance data clarity, consistency, and professionalism for improved presentation and management.


(This Steps are for MacOS)
# Step 1: Autofit Column and Row Widths for Optimal Readability
Begin by ensuring that every column and row is perfectly sized to display all content without any
truncation or awkward spacing. This step improves the readability of data, enhancing visual clarity
and professionalism in your spreadsheet.
Command for Columns:
• Press Control + Option + Command + I to auto-fit all selected columns. This command
expands or contracts the width of each column to fit the widest cell content automatically.
Command for Rows:
• Press Control + Option + Command + A to auto-fit row heights, allowing all text to be
visible without cutting off any information.
This step ensures that every entry in your data is immediately visible, reducing the need for manual
adjustments.
# Step 2: Remove Text in Parentheses to Clean Client Names
Cleaning up client names by removing unnecessary text inside parentheses is vital for clarity and
uniformity, especially when dealing with long names or added descriptions. To do this efficiently,
use Find and Replace with a special wildcard to target any text within parentheses.
1. Shortcut for Find and Replace: Press Command + Shift + H to open the Find and
Replace window.
DWBI LAB PRACTICAL
2. 3. In the Find box, enter “(*)” to specify that all text within parentheses should be removed.
Leave the Replace box empty, then click Replace All.
This transformation eliminates distracting details and presents the data in a clean, concise format.
# Step 3: Convert Text to Lowercase for Consistency
For uniformity, convert all client names to lowercase. This approach creates a professional and
consistent look, particularly when working with large datasets with varied text formats.
1. 2. Create a New Column adjacent to your existing data.
In the first cell of this column, type =LOWER(cell), replacing “cell” with the actual cell
reference you wish to transform. For instance, if your data begins in cell B2, you would type
=LOWER(B2).
3. Press Enter, and then drag the formula down to apply it to all cells in the column.
To remove the formula and keep only the lowercase text, select the entire column, press
Command + C to copy, then use Command + Shift + V to paste as values (or choose Paste
Special > Values from the Edit menu).
# Step 4: Trim Extra Spaces and Capitalize Names for a Polished Appearance
Remove excess spaces and apply proper capitalization to each word, ensuring a neat and readable
dataset.
1. 2. 3. Insert a New Column and type =TRIM(cell) to remove any extra spaces.
Combine with =PROPER(cell) to capitalize the first letter of each word.
For example, enter =PROPER(TRIM(B2)) to apply both formatting rules at once.
This approach eliminates inconsistencies in spacing while standardizing name formatting.
# Step 5: Split Text into Separate Columns for Clarity
Separate information like department names and regions, currently stored in one cell, into distinct
columns. This practice facilitates targeted data analysis and cleaner organization.
1. Select the entire column with the combined information.
2. Go to Data > Text to Columns.
3. Set the delimiter to an underscore (_) and click Finish.
Each component of the original text will now appear in its designated column, making your data
more organized and accessible.
# Step 6: Remove Duplicate Entries to Prevent Redundancy
Prevent data repetition by removing duplicate entries in your dataset.
1. 2. Select the Entire Table to apply duplicate detection across all columns.
Go to Data > Remove Duplicates and confirm your selection.
This action helps maintain data integrity by ensuring that each entry is unique.
DWBI LAB PRACTICAL
# Step 7: Fill Blank Cells with 'N/A' for Consistency
Avoid confusion caused by blank cells by replacing them with “N/A,” indicating missing data.
1. Select the dataset, then go to Edit > Find > Go to Special and choose Blanks to select all
empty cells.
2. Type N/A in the formula bar and press Command + Return to apply it to all selected blank
cells simultaneously.
This small step enhances your dataset’s readability and prevents potential errors during analysis.
# Step 8: Handle Errors in Formulas Using IFERROR
Ensure calculations are error-free by using IFERROR to manage potential issues.
1. In cells with calculations, wrap the formula with =IFERROR(formula, "N/A").
This approach replaces any error result with “N/A,” keeping your data clean and error-free.
This function is essential in large datasets where specific cells may generate errors, as it replaces
those errors with meaningful placeholders.
# Step 9: Format the Header Row for Emphasis
Make your header row stand out by bolding text and applying contrasting colors.
1. 2. Select the Header Row and press Command + B to bold the text.
Use the Home tab’s Fill Color and Font Color options to apply contrasting colors, such as
dark blue for the background and white for the text.
This step enhances the visual appeal of your data and makes column headings easy to identify.
# Step 10: Remove Gridlines for a Polished Look
Turn off gridlines to give your worksheet a clean, professional appearance.
1. 2. Go to View > Gridlines to toggle them off, or use the shortcut Option + Command + U.
The absence of gridlines makes your data more visually appealing, particularly in
presentations.
