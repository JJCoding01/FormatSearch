Format Search
==============

## Description

*Format Search* is a Sublime Text 3 package designed to take a list of part numbers and format them for different types of searches.

The search formats that *Format Search* is designed for is searching a SolidWorks® PDM vault for SolidWorks® files, and WorkWise ERP list search.

This package is not designed to be integrated with the search tools, to display results, but merely be a tool to quickly format a list of part numbers for inputting into the search tool.

The formatting takes place internally and copies the result to the clipboard to make it easy to paste results into the search tool.

There are five different search formats that are created. These five are

 - **Drawing** space delimited list with *.SLDDRW* suffix to every part number
 - **Part** space delimited list with *.SLDPRT* suffix to every part number
 - **Assembly** space delimited list with *.SLDASM* suffix to every part number
 - **TCM** comma delimited list with each part number in double quotes
 - **Plain:** no changes, simple space delimited list of raw part numbers

## Usage
The search formats are listed under context menu under the menu *Format Search*, as well as in the command palette. To use the command palette, search for *FormatSearch:* and you will be presented with the different formatting options.

If there are part numbers pre-selected, that selection will be used, otherwise the current region will be used.

## Examples

The following examples assume the following part numbers are under the cursor.

```
123452
239084
029382
```
Activating the different formats will give the following results

 - **Drawing:** `123452.SLDDRW 239084.SLDDRW 029382.SLDDRW`
 - **Part:** `123452.SLDPRT 239084.SLDPRT 029382.SLDPRT`
 - **Assembly:** `123452.SLDASM 239084.SLDASM 029382.SLDASM`
 - **TCM:** `"123452", "239084", "029382"`
 - **Plain:** `123452 239084 029382`

## License
MIT license.

## Credits
Thanks to [Karolis Astrauka](https://github.com/astrauka) for his blog article *[sublime text plugin development basics](http://engineering.vinted.com/2016/06/27/how-to-write-sublime-plugin/)*
