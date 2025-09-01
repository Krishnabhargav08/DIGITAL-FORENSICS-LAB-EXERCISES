# Experiment 1: Evidence Acquisition Using FTK Imager

## Aim
To capture RAM data and create a forensic disk image using FTK Imager.

## Requirements
- FTK Imager
- Windows Operating System

## Description
- FTK Imager creates bit-by-bit forensic images of hard drives, partitions, and other storage media, preserving the original data, including file slack and unallocated space, without altering it.
- It allows investigators to preview files, folders, and forensic images on various media types, supporting analysis tasks like keyword searching, metadata extraction, and file type identification.
- The tool generates MD5 and SHA1 hash values to verify the integrity of forensic images, ensuring they remain unchanged and admissible in court.

## Acquiring Volatile Memory (RAM) Using FTK Imager

### Step-1
Right-click on FTK Imager and run as Administrator.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im1.png)

### Step-2
On the top-right menu bar, click **File** and select **Capture Memory** from the drop-down list.

![(images/step2.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20Im2.png)

### Step-3
A box will appear. Select the destination path for your file and provide the file name with a `.mem` extension. Pagefile and AD1 file options are optional.

![(images/step3.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20Im3.png)

### Step-4
A green progress bar will indicate the capture status. The time taken to capture the RAM depends on the RAM size. After completion, the memory dump file will be available in the destination folder.

![(images/step4.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20Im4.png)

After installation the report will be appeared in file explorer like .mem

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20Im5.png)

## Acquiring Non-Volatile Memory (Disk Image) Using FTK Imager

### Step-1
On the top-right menu bar, click **File** and select **Create Disk Image** from the drop-down menu.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im6.png)

### Step-2
In the dialog box, choose the source evidence type (e.g., Physical Drive, Logical Drive, Image File, or Contents of a Folder)

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im7.png)

### Step-3
Select the drive you want to image and click **Finish**.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im8.png)

### Step-4
In the "Create Image" dialog, click **Add** to define the image type.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im9.png)

### Step-5
Select the image type from the dialog box (Raw, SMART, E01, AFF). E01 is recommended.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im10.png)

### Step-6
Fill in the case information and click **Next**.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im11.png)

### Step-7
Choose the destination folder and provide a file name for the image.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im12.png)

### Step-8
Set options like compression and splitting size, then click **Finish** to start the imaging process.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/5c1b9cc92b4a1d3933d232db5d2a58fcabd9b0db/images/Ex-1%20im13.png)

FTK Imager will display progress along with hash values. The imaging process may take time depending on the drive size. After completion, FTK Imager verifies the hash values automatically to maintain forensic integrity. Finally, the hash values are matched.
