# Experiment 2: Recover Deleted or Damaged Files from a Storage Device Using TestDisk

## Aim
To recover lost partitions and deleted files using TestDisk.

## Requirements
- TestDisk
- Windows Operating System

## Description
- TestDisk recovers lost or deleted partitions by scanning storage devices to locate and rebuild partition tables, supporting formats like FAT, NTFS, ext2/ext3/ext4, and GPT.
- It repairs corrupted filesystems, such as fixing FAT/NTFS boot sectors or rebuilding MBR, enabling non-booting disks to become bootable again.
- TestDisk includes PhotoRec, a file carving tool that recovers unfragmented files from various storage devices by identifying file signatures, independent of the filesystem.

## Steps

### Step-1
Launch the TestDisk tool and in the terminal window, select “Create” to make a new log file and press Enter.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im1.png)

### Step-2
TestDisk will list available disks (HDDs, SSDs, USB drives). Use the arrow keys to highlight the disk you want to analyze and Press Enter.

![(images/step2.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im2.png)

### Step-3
TestDisk usually auto-detects the partition table (Intel/PC, EFI GPT, Mac, etc.). Verify and press Enter.

![(images/step3.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im3.png)

### Step-4
Analyze the current partition structure, from the terminal select Analyse and press enter.

![(images/step4.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im4.png)

### Step-5
After analysis you will be asked to perform Quick search select it and press Enter.

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im5.png)

### Step-6
TestDisk scans the disk and lists lost partitions.

![(images/step6.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im6.png)

### Step-7
Press “P” to view the list of files and “C” to copy the files.

![(images/step7.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im7.png)

### Step-8
If Quick Search does not find your partition/files, select “Deeper Search” and Enter. This takes longer but finds more recoverable partitions.

![(images/step8.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im8.png)

### Step-9
Once you are confident the partition is correct, select “write” and press Enter.

![(images/step9.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im9.png)

### Step-10
Confirm the operation by pressing “Y”. This will write partition table to your disk.

![(images/step10.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/16b1147bcb109484f40eeb2ca02cfa07e0376c71/images/Ex-2%20im10.png)
