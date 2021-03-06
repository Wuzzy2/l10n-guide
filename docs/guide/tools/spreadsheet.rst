
.. _../pages/guide/tools/spreadsheet#using_csv_and_your_spreadsheet_to_edit_translations:

Using CSV and your Spreadsheet to edit translations
***************************************************

A CSV (Comma Separated Value) file is one in which each field or cell is
separated by a comma (or another character) and each record or line is
separated by a newline.

When using CSV files generated by :ref:`po2csv <toolkit:po2csv>` you will find the data
as follows:

=========  =============================================================================================================================================================================================
 Column     Description                                                                                                                                                                                   
=========  =============================================================================================================================================================================================
  A         contains the location information from the PO file.  This is sometimes usefull for working out what the message is used for as its location and the name of the message can provide clues.    
  B         contains the original or English text                                                                                                                                                         
  C         you add your translations to this column                                                                                                                                                      
=========  =============================================================================================================================================================================================

.. _../pages/guide/tools/spreadsheet#notes:

Notes
=====

Preserve filenames, do not change the case of the filename.  Return files in a
ZIP archive in the same order and directory structure.  This is important
because the reverse process, coverting CSV to PO is made easier if you do not
change these.

.. _../pages/guide/tools/spreadsheet#how_to_open_a_csv_file:

How to open a CSV file
======================

When opening a CSV file you will be presented with a number of questions.  Here
are the answers you should provide:

.. _../pages/guide/tools/spreadsheet#openoffice.org_2.0:

OpenOffice.org 2.0
------------------

- In the text import dialog.  Ensure that the character set in 'Unicode UTF-8'.
  Under 'Separator options' ensure that the 'Separated by' radio button is
  selected and the 'Comma' is checked.  The text delimeter should be " (double
  quotes).
- Check to see that the import wizard has identified the 3 columns correctly
- Click OK

.. _../pages/guide/tools/spreadsheet#microsoft_excel_97/2000:

Microsoft Excel 97/2000
-----------------------

There is a problem with Microsoft Excel 97 and 2000 in that it opens a UTF-8
file as if it is ASCII.  Excel does save CSV files correctly, if the encoding
of the opened file is retained, but Excel by default does not retain the
encoding.  Some success has been had using `XSLGEN
<http://www.ensoft.de/xlsgen/xlsgen.htm>`_ (edit the xslgen.bat file to reflect
the location of your installation of Excel) to open UTF-8 CSV files correctly
in Excel. 

.. _../pages/guide/tools/spreadsheet#getting_the_most_from_your_spreadsheet:

Getting the most from your spreadsheet
======================================

Initially the first column will stretch across the page as it contains a large
amount of data, but you cannot see or work with this data.  Therefore do the
following:

- **Adjust the column widths** -- 5" works well as you can then see both the
  original and translation clearly.
- **Adjust the cell formating** for the first column to allow the insertion of
  automatic line breaks (this will cause the data to wrap within the column and
  make it all readable) this also allows for automatic hyphenation which will
  then hyphenate long words.  The result of this step is that you can now read
  all data in column one as the rows will become larger to accommodate this
  information.
- You can repeat this process for other columns but then messages will wrap
  differently to how they appear in the translation.  Do this only if you
  really don't have space or otherwise look at text shrinking options.

Each Spreadsheet application will achieve the above in a slightly different
way.  Here are specific instructions.

.. _../pages/guide/tools/spreadsheet#openoffice.org:

OpenOffice.org
--------------

- Right click on the header of Column A.  Select "Column Width". Type in a
  value in the "Width" field.
- Right click on the header of Column A.  Select "Format Cells...", then select
  the "Alignment" tab.  Now under Properties enable "Wrap text automatically"
  and "Hyphenation active".
- If you can't see column B or C clearly.  Select the header of the column.
  Select "Format Cells...", then select the "Alignment" tab.  Now under
  Properties disable "Wrap text automatically" and enable "Shrink to fit cell
  size"

.. _../pages/guide/tools/spreadsheet#microsoft_excel:

Microsoft Excel
---------------

FIXME
