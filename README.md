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
**Step-1:** Download the [GPG Keygen](https://gpgtools.org/)

**Step-2:** Install the downloaded .dmg file.

**Step-3:** 
