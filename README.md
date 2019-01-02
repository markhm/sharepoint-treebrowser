SharePoint Tree Browser (DK-DA version)
======================
_Have your SharePoint libraries become slightly unorganised?_

This tool visualises exported metadata exported from one or more SharePoint libraries. It will help you understand 1) where documents are, 2) which structure and governing rules are missing and 3) what needs to be done to bring a bit of order and keep your teams productive. 

_Currently, the SharePoint Tree Browser only supports a limited number of metadata columns in Danish, see below._

_If this project is interesting to you, don't hesitate to get in touch._

## Features and how to use
The SharePoint TreeBrowser features:
- Tree-based visualisation of documents in one or more SharePoint libraries
- Seamless zooming in/out to quickly understand large data structures and their relevant details
- Selecting Degree-of-Interest depth, to show more or less nodes surrounding the selected note
- Searching for documents based on keywords, expanding the tree to show search results
- Turn on coloring layers to visualise:
  - **Document age** - Change date minus Creation date
  - **Modification year**
  - Metadata top 10 - Most frequently used metadata elements per column
- Currently supports the following Danish metadata colums:
  - **Navn** - Name
  - **Sti** - Tree position
  - **Oprettet** - Creation date
  - **Oprettet af** - Created by
  - **Ændret** - Change date
  - **Ændret af** - Changed by
  - **Arbejdspakke** - Work package
  - **Produkt** - Product
  - **Produkt type** - Product type
  - **Flyt til arkiv** - Archived (Y/N)
  - **Forretningsenhed** - Business unit
  - **Indholdstype** - Content type
Please let me know if you would like to see other languages supported, in particular: send me the names of the metadata columns. 

How to use:
- Observe that the tree at the first level shows the repository, followed by the particular library at the next level.
- Use the depth slider to show a larger part of the tree, or select a particular node to uncover a deeper part of the tree.
- Click various nodes to see the tree parts expand.
- Pan by holding the left mouse button (not on a node) and moving.
- Zoom by holding the right mouse button and moving up or down.
- Double click to fit to zoom.
- Select a metadata column (Group) and turn on the visualisation (tick box) and observe the most used elements in the legend.
- Reset by selecting the root node, setting depth to 1 and clicking the Center button.
- Enter a keyword in the search box, click the Expand tick box to expand.
- Click the Center button to center the visualisation in case you loose perspective.

## Prerequisites and acknowledgements
Requires Java 1.8 or higher. 

The SharePoint Tree Browser was developed on a display with a 1680 by 1050 resolution. Screen options or buttons might have moved or may be hidden when you are running on a different resolution. 

Based on <a href="http://prefuse.org">prefuse</a>, a visualisation library for Java developed by <a href="http://jheer.org">Jeffrey Heer</a>.

## Preparing data and running
Prepare metadata you would like to visualise as follows:
  1. Create a custom view in the SharePoint library where all (relevant) columns are selected
  2. Export the metadata to Excel and save as xlsx.
  3. Open the xlsx in Excel and Save as xls (older data format).
  4. Drop the xls file in a subdirectory called 'data'
  5. Start the jar file with 'java -jar [filename]'
  
## Download
The SharePoint Tree Browser is available as executable jar via [this link](https://github.com/markhm/sharepoint-treebrowser/blob/master/binaries/SharePointTreeBrowser-20190102.jar).

## Version history
- 20190102 - Testing the release process and the first release.

## Known issues
- Search does not support looking up consecutive keywords well. Change the depth on the depth slider to change to update the visualisation to the new search results, or restart the application.
- When running the ActionList, the prefuse visualisation framework sometimes throws a NullPointerException, which can be ignored.
