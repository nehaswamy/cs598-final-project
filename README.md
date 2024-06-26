# Set Up
1. Clone this project using "git clone https://github.com/nehaswamy/cs598-final-project.git" (HTTPS) or "git clone git@github.com:nehaswamy/cs598-final-project.git" (SSH)
2. Go to [Google Colab](https://colab.research.google.com/)
3. You should be prompted to open a notebook. Go to "Upload" and then browse for the DL4H_Team_101.ipynb file or drag it.
4. Go to Google Drive to locate your new Colab file.
5. In the Colab file, change the global variable variable "root" to the path of the folder containing your Colab file. This folder will also hold any other files and folders needed to run this project. 

# Steps to Access and Load the Data
1. Request access to the [ADNI dataset](https://ida.loni.usc.edu/collaboration/access/appLicense.jsp)
2. Once you receive an email confirming your access, login with your credentials [here](https://ida.loni.usc.edu/login.jsp?project=ADNIhttps://ida.loni.usc.edu/login.jsp?project=ADNI)
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
17. Convert the images to JPG (see [instructions](https://medium.com/@vivek8981/dicom-to-jpg-and-extract-all-patients-information-using-python-5e6dd1f1a07d))
18. Create a folder called "data" in the same folder that holds your Colab notebook in Google Drive.
19. Within the "data" folder, create a folder called "train".
20. Create a folder called "AD" within the "train" folder and move the JPG images there.
21. Repeat steps 3-17, this time with "CN" data (i.e., check the "CN" box in the "Research Group" section, create a folder called "CN" within your "train" folder in Google Drive, and move the converted JPG images to the "CN" folder.)
22. Create an empty "val" folder with empty "AD" and "CN" folders.
23. If you have not already, in the notebook, change the variable called "root" to the path of the folder containing your Colab file and "data" folder (for instance, mine is '/content/drive/MyDrive/CS_598_Final_Project'.)

# Main Model Results
Metric     | Result   |
| -------- | -------- |
Accuracy   | 0.517241 |
F1	       | 0.681818 |
Precision  | 0.517241 |
Recall	   | 1.000000 |
ROC AUC	   | 0.500000 |
