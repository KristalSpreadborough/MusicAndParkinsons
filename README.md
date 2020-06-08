# Music And Parkinson's Disease
<br>Please cite this code as:
<br>Spreadborough, Kristal (2020) Music and Parkinson's Disease (Version 1.0) [Source code]. https://github.com/KristalSpreadborough/MusicAndParkinsons
<br>
<br>
This code was used to clean metadata used for a systematic review of research into Music and Parkinson's disease.
First, relevant fields from an XML file downloaded from PubMed were extracted using the following xslt style sheets: 
<br>stylesheetJournal.xslt
<br>stylesheetJournalDate.xslt
<br>stylesheetJournalIssue.xslt
<br>stylesheetTitleLanguage.xslt
<br>
<br>
These fields were written to individual csv's and then merged into a single csv using the commands found in:
<br>WritingXMLtoCSV200608.txt
<br>
<br>
The resulting csv of PubMed data along with csv's from Scopus and Web of Science were then merged into a master file with duplicates removed using this code: 
<br>MergFilesRemoveDuplicates200608.ipynb
<br>
<br>
Finally, inclusion/exclusion criteria for each publication were checked in this master file using the following code:
<br>CheckingForKeyWords200608.ipynb
<br>
<br>
NOTE: For the PubMed xml data, the "Abstract" field was added to the master file by hand since it was difficult to extract via xslt style sheet. This was because the Abstract field was often  broken up into different sections and these were difficult map to specific publications. 
