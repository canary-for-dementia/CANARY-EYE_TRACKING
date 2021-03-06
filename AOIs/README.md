This Folder contains the following subfolders:

* CookieTheft/ contains the following files:
    * CookieTheft_CANARY_Setup_AOIs_blue.JPG is a graphical representation of the AOIs defined for the CookieTheft task. **this file was created manually**
    * The file All_AOIs.txt contains the coordinates of the vertices for each of the AOIs. This file needs to be passed to GenerateAuxiliaryFiles.R as input for ET pre-processing pipeline. **this file was created manually**

* Reading/ contains the following files:
    * Reading_AOIs_basicInfo.txt contains the information, for each word in the reading task including wordID, lineID, sentenceID and number of characters. **this file was created manually**
    * GenerateReadingAOIs.R is the script that generates the boundingboxes coordinates for each word in the Reading task, which will be used to generate reading features. This script takes as input Reading_AOIs_basicInfo.txt, as well as the reading task screenshot found under AOIs > Tasks-Screenshots
    * Reading_AOIs_basicInfo.txt is the file that contains the bounding boxes and basic info for each of the words in the reading task, this file is used by ReadingTaskFeatures > ReadingTaskScript.py to generate reading features. **this file is generated by GenerateReadingAOIs.R**
    * Reading_AOIs.png: is a visual representation of the word's bounding boxes. **this file is generated by GenerateReadingAOIs.R**

* Tasks-Screenshots/ contains exact screenshots for each of the tasks in the CANARY battery. These screenshots correspond pixel-by-pixel to what participants see during the experiment, and are used to define the AOIs (either manually for CookieTheft or computationally for Reading Task) 
