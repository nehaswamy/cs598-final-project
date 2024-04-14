# Steps to Access and Load the Data
1. Request access to the ADNI dataset (https://ida.loni.usc.edu/collaboration/access/appLicense.jsp)
2. Once you receive an email confirming your access, login with your credentials here: https://ida.loni.usc.edu/login.jsp?project=ADNIhttps://ida.loni.usc.edu/login.jsp?project=ADNI
3. Go to Download > Image Collections > Advanced Search
4. Copy and paste the list of subjects in "subjects.txt" in the "Subject ID" field.
5. In the "Research Group" section, select AD.
6. In the "Study/Visit" section, select all the checkboxes that match "ADNI1/GO Month X," where X is a number.
7. Check off "T1" in the "Weighting" section.
8. Click "Search."
9. Check "Select All" and click "Add to Collection."
10. Enter a name for your collection and click "OK."
11. Go to Data Collections.
12. Click "My Collection" > *name of your collection* > "Not Downloaded"
13. Check the "All" box.
14. Click "1-Click Download"
15. Click "Zip File 1" to download a zip file of the data.
16. Unzip the file.
17. Convert the images to JPG (see https://medium.com/@vivek8981/dicom-to-jpg-and-extract-all-patients-information-using-python-5e6dd1f1a07d for instructions.)
18. Create a folder to hold your JPG files.
19. Within that folder, create a folder called "train".
20. Create a folder called "AD" within the "train" folder and move the images there.
21. Repeat steps 3-17, this time with "CN" data (i.e., check the "CN" box in the "Research Group" section and create a folder called "CN" within your "train" folder in Google Drive that holds these images.)
22. Create an empty "val" folder with empty "AD" and "CN" folders.
