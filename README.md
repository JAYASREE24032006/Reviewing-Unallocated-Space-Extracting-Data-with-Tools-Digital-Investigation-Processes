# EX-5 : REVIEWING UNALLOCATED SPACE EXTRACTING DATA WITH TOOLS DIGITAL INVESTIGATION PROCESS
## AIM :
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS :
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM :
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS :
### Step 1 (Acquire Evidence Image) :
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool) :
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space) :
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data) :
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM :
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT :
Unallocated Space Analysis and Extracted Data Report

<img width="935" height="744" alt="image" src="https://github.com/user-attachments/assets/4a24164b-33b3-4df9-ad49-1daabf798365" />

<img width="1898" height="1132" alt="image" src="https://github.com/user-attachments/assets/7f385678-d1c1-4647-85dc-a6b1fbbb876f" />

<img width="937" height="736" alt="image" src="https://github.com/user-attachments/assets/848db8f4-7a20-41f9-af51-5db25dbfa3cf" />

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/b8d1e6e5-8c44-45aa-9c35-1080cc926533" />

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/7e5ebae1-3220-48d7-9f9c-a4604580df7e" />

<img width="1917" height="1199" alt="image" src="https://github.com/user-attachments/assets/917f2f54-eae9-4d60-88d0-1954839ab8ca" />

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/6e1864c5-b13e-463e-a9aa-844fd31222f9" />

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/5ee5f8eb-ecd8-4762-be5a-9d98d7c90fe0" />

<img width="1354" height="392" alt="image" src="https://github.com/user-attachments/assets/798c7733-d881-4494-ac9d-33297504902f" />

<img width="1919" height="1050" alt="image" src="https://github.com/user-attachments/assets/86d2263d-93bf-4629-8a97-833abdf2a365" />

<img width="1447" height="770" alt="image" src="https://github.com/user-attachments/assets/94724e27-356f-43d6-8d9a-58227a328eeb" />


## RESULT :
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

