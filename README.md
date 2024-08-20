# Create PGP Certitificate for Boomi with Expiry Date

## Problem Statement
When we create a PGP Certificate in Boomi, the Expiry Date isn't set by Boomi. Some boundary systems require the expirt date to be set, as per their information security protocol.

## Analysis
This is a Boomi product limitation.

## Solution
**Step-1:** Generate the PGP Certificate in an external tool/software. Keep a note of the Password/Passphrase, as it will be required in a later step.

**Step-2:** Export the Public Key and the Private Key from the external tool/software, in .asc format, and store it in your computer.

**Step-3:** In Boomi, create a "PGP Certificate" compinent. Select "Import" option. Import the Private Key (generated in the first step), put the Password/Passphrase, and click "Finish".

**Step-4:** Share the Public Key with the buondary system team through a secure channel.

## Generate PGP Certificate in macOS
**Step-1:** Download the [GPG Keychain](https://gpgtools.org/) application.

**Step-2:** Install the downloaded .dmg file.

**Step-3:** Select the "New" button to create the new certficate. A pop-up window will open.
![image](https://github.com/user-attachments/assets/5c52ef22-7713-4b4f-88e3-06d6e94c1954)

**Step-4:** Put the values as per your requirements, and click on the "Create Key" button. Please find a sample screenshot below.
![image](https://github.com/user-attachments/assets/df19ce4e-6952-4a72-b5de-0e836744b486)

**Step-5:** Select the newly generated certificate, and click on the "Export" button. A pop-up window will open.

**Step-6:** Provide the desired file name and the folder location where the keys needs to be saved. To download the Public Key, click on the "Save" button. To download the Private Key, select the "Include secret key in exported file" checkbox, enter the Password/Passphrase when prompted, and click on the "Save" button.
![image](https://github.com/user-attachments/assets/118169e3-1856-43e0-b91a-ff462350c15e)
