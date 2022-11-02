# Formal-Verification-of-the-WirelessHART-Protocol
This repository contains the Tamarin Prover files for the paper "Formal verification of the WirelessHART Protocol - Verifying Old and Finding New Attacks"

# Files
This repository contains Tamarin models for the WirelessHART protocol.
To keep the files manageable the model has been split into parts mapping to different parts of the WirelessHART specification.

1. **wirelessHART\_e2e.spthy**
2. **wirelessHART\_join.spthy**
3. **wirelessHART\_key\_change.spthy**
4. **wirelesshART\_dlpdu.spthy**

# Requirements
This model was created and tested with Tamarin Prover version 1.4.1. 
The latest version of Tamarin Prover can be found and downloaded [here](https://tamarin-prover.github.io/manual/book/002\_installation.html).
It is also useful to have the Tamarin Prover manual that can be found [here](https://tamarin-prover.github.io/manual/index.html).

# Running Instructions

To run Tamarin from the terminal run the following command (you can of course change the .spthy file):
`tamarin-prover wirelessHART_e2e.spthy`
Then you can prove properties with a command like:
`tamarin-prover wirelessHART_e2e.spthy --prove=message_authentication_UC`

Or use the Tamarin web-based graphical user interface run:
`tamarin-prover interactive .`
And open `http://127.0.0.1:3001` in your web browser.
