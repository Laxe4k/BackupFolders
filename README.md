# Backup Script - by Laxe4k

## Description
This batch script allows you to back up specified folders by compressing them into a 7z file. It also checks if 7-Zip is installed and installs it if necessary.

## Features
- Creates a compressed backup file using 7-Zip.
- Allows you to specify the backup folder and folders to be backed up.
- Provides options to change the backup folder, compression level, and add folders to be backed up.
- Checks and installs 7-Zip if necessary.

## Script Steps

1. **Initialization**:
   - Configures encoding to UTF-8 and sets necessary variables for the backup.

2. **Preparing the Backup Folder**:
   - Reads the backup folder path from a text file (BackupDir.txt) or prompts the user to specify it.

3. **Checking for 7-Zip**:
   - Verifies if 7-Zip is installed and installs it via winget if necessary.

4. **Main Menu**:
   - Displays a menu with options to perform a backup, change the backup folder, change the compression level, add folders to be backed up, or quit.

5. **Adding Folders**:
   - Allows the user to add folder paths to be backed up into a text file (Folders.txt).

6. **Backup**:
   - Creates necessary folders for temporary backup.
   - Copies files from specified folders into the temporary backup folder.
   - Compresses the temporary backup folder into a 7z file with the specified compression level.
   - Moves the 7z file to the backup folder.

7. **Changing the Backup Folder**:
   - Allows the user to specify a new path for the backup folder.

8. **Changing the Compression Level**:
   - Allows the user to choose the compression level for 7-Zip.

## Usage

1. **Running the Script**:
   - Double-click the batch file to run the script.
   - Follow the on-screen instructions to configure and perform the backup.

2. **Command Line Options**:
   - Use the `-auto` argument to run the backup automatically without displaying the menu.

## Notes
- Ensure that 7-Zip is installed or that winget is available for automatic installation.
- The paths of the folders to be backed up should be specified in the `Folders.txt` file.
