Updated 18/04/2018 by Matthew KELLY

# UFED Cellebrite images by hash report
A Python script to read a CSV file exported from Griffeye to find matching MD5 values and create report(s) with subsequent Categories.


* FFMPEG.exe must be located in the following location on the same PC and in the root, i.e. C:\FFMPEG.exe.
* Export a CSV file containing what you want from UFED Cellebrite, must include Category and MD5 as these are used by the script.
    - Can also export Tags as this can be used by the script as a comment.
* Open file download inside UFED Physical Examiner.
* Run script by selecting Python -> Run Script...
* This will cause the selection screen to be displayed. 
    - File and Folder Dialog boxes cannot be displayed from UFED Cellebrite as it is a Sandboxed environment.
* Enter the:
    - full folder and filepath of CSV file including extension.
    - Folder for Report. _**Note**: this must be a folder that does not exist, as the script will create the folder._
    - Enter the intended name for the Report(s)
    - There is an option to create one large report or individual reports for each category in the selection box.
* The script will run for Images first and then Videos.
* Once completed check the HTML report.Copy and paste folder locations relevant to the following user choice:
    - Accessible, e.g. Downloads, DCIM.
    - Application Specific, e.g. android.com/WhatsApp.
    - Non-accessible, e.g. DCIM/.thumbnails.
    - All remaining images/videos will be shown under the sub-title 'Unknown'
* Refresh the report and repeat the previous step until satisified with sub-categorisation.
