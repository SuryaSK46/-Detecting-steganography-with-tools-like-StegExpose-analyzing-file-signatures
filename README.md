# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands

## OUTPUT:
List of Images with Steganography Detection Scores and File Signature Details
1.Install and Set Up StegExpose • Download the StegExpose .jar file from the official repository. • Ensure Java Runtime Environment (JRE) is installed. • Run the tool on an image or a folder of images:\
• The output will list detection scores and a "suspect" verdict if steganography is found.

2.Scan Individual Files • Run StegExpose on a single image:
The tool uses statistical analysis methods like RS analysis, Sample Pair analysis, and Chi-square attack to detect hidden content.

3.Analyze File Signatures • Use Linux commands to verify the file's true format:
Every file type has a magic number (e.g., JPEG files start with FFD8). Comparing the actual signature with the file extension helps identify mismatches or embedded file tricks.

4. Cross-Check File Behavior • Rename the file (e.g., mv suspicious.jpg suspicious.zip) and try extracting it:

o Sometimes, files are disguised (e.g., a ZIP file hidden as a JPG), and this trick helps uncover such embedded archives.

5.Optional: Use Other Tools


o Tools like binwalk, stegsolve, or zsteg can be used for deeper analysis, especially for PNG files or binary dumps.


<img width="478" alt="image" src="https://github.com/user-attachments/assets/51e0bcad-b689-48cb-bccf-c8afc4bf2b19" />


<img width="540" alt="image" src="https://github.com/user-attachments/assets/31bda16d-f5bc-4820-b2ed-9fbd299816a3" />




<img width="614" alt="image" src="https://github.com/user-attachments/assets/64215dbe-8643-4665-8836-e762e41fe86c" />


<img width="627" alt="image" src="https://github.com/user-attachments/assets/cf538c78-40fe-4f75-9742-33885051e2e0" />



<img width="619" alt="image" src="https://github.com/user-attachments/assets/d3c83910-4b9d-4692-8def-dfbcdaf1b3e9" />
















## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
