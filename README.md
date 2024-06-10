# BMCacheHunter

## What is BMCacheHunter?

BMCacheHunter serves as both a Threat Hunting and Digital Forensics tool. Originally developed by Nir Saias, Yossi Sassi, and Rotem Lipowitch as a Proof of Concept for BSIDES 2021 TLV ([Watch the presentation](https://youtu.be/60Y07kdcIcw)), it specializes in collecting BMC files from domain computers.

![BMC Image](https://user-images.githubusercontent.com/21937074/126483231-2a5f13b0-67a9-4e90-9117-cee34d4336b5.png)

The process involves formatting the BMC files into JPG collages and extracting text using an OCR mechanism (Tesseract).

![OCR Image](https://user-images.githubusercontent.com/21937074/126483187-71eaeb4c-d7a5-41d0-85ed-0c538d894c2c.png)

This tool offers full customization, enabling users to search for specific strings within the RDP "history" of computers within the domain.

## SETUP

### Installing
1. Install Tesseract located in the "BSIDES-BMCacheHunter\tools" folder.
2. Add the Tesseract executable to the Environment path.
3. Populate the list of computers you wish to examine in the `Computer_List.txt` file.
4. Edit the Indication of Compromised in the `IOC.txt`.

### Execute

```powershell
PS > .\BMCacheHunter.ps1
```

```powershell
PS > .\BMCacheHunter.ps1 -ComputerList .\Computer_list.txt -IOCList .\IOC.txt
```

## Licensing

For licensing details and terms of use, refer to the [LICENSE](LICENSE) file.

## Contact Us

For further inquiries, visit [10Root Cyber Security](https://10root.com).
