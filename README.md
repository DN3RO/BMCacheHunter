# BMCacheHunter

# What is BMCacheHunter?
BMC Cache Hunter can be used as a Threat Hunting as well as for a Digital Forensics tool. Written by Nir Saias, Yossi Sassi and Rotem Lipowitch as a PoC for BSIDES 2021 TLV.
Collecting BMC files from the domain computers.
![image](https://user-images.githubusercontent.com/21937074/126483231-2a5f13b0-67a9-4e90-9117-cee34d4336b5.png)

Formating the BMC to JPG collages and extract the text using an OCR mechanism (Tesseract).
![image](https://user-images.githubusercontent.com/21937074/126483187-71eaeb4c-d7a5-41d0-85ed-0c538d894c2c.png)

The tool is fully adjustable and will let you search any string you like in the RDP "history" of computers in the domain.

# SETUP

# Installing
1. Install Tesseract located in the "BSIDES-BMCacheHunter\tools" folder.
2. Add Tesseract executable to the Environment path.
3. Populate the computers you want to examine in the Computer_List.txt file.
4. Edit Indication of Compromised in the IOC.txt

# Execute

PS > .\BMCacheHunter.ps1

PS > .\BMCacheHunter.ps1 -ComputerList .\Computer_list.txt -IOCList .\IOC.txt

# Licensing


# Disclaimer

# Contact Us
