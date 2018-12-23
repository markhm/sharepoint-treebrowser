SharePoint TreeBrowser
======================
_Has your SharePoint library become slightly unorganised over time?_

This tool visualises exported metadata exported from one or more SharePoint libraries. It will help you understand 1) where documents are, 2) which structure or governing rules are missing and 3) what needs to be done to bring a bit of order and keep your teams productive. 

_This page and the release of the SharePoint TreeBrowser is work in progress._

## Features
The SharePoint TreeBrowser features:
- Tree-based visualisation of documents in one or more SharePoint libraries
- Seamless zoom in/out to quickly understand large data structures and their relevant details
- Currently supports the following Danish metadata colums:
  - Oprettet (Creation date)
  - Oprettet af (Created by)
  - Ændret (Change date)
  - Ændret af (Changed by)
  - Arbejdspakke (Work package)
  - Produkt (Product)
  - Produkt type (Product type)
  - Flyt til arkiv (Archived Y/N)
  - Forretningsenhed (Business unit)
  - Indholdstype (Content type)
  
## Prerequisites and acknowledgements
Requires Java 1.8 or higher. 

Built on <abbr title="https://prefuse.org">prefuse</abbr>, a visualisation library for Java developed by <attr title="http://jheer.org">Jeffrey Heer</attr>. 

## Preparing data
Prepare metadata you would like to visualise as follows:
  1. Create a custom view in the library where all (relevant) columns are selected
  2. Export the metadata to Excel and save as xlsx.
  3. Open the xlsx in Excel and Save as xls.
  4. Drop the xls file in a subdirectory called 'data'
  
## Download and run
The SharePoint TreeBrowser is available as fat jar via:@@. Currently, versions are 



