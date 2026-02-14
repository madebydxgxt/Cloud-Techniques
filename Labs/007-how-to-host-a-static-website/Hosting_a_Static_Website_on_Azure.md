# Hosting a Static Website on Azure (Blob Storage)

This lab demonstrates how to host a simple static website using Azure Storage and Blob Service.

## Watch me build this lab
https://www.loom.com/share/95c44fe345c64003a5e720a0336ec0ba

**What this video shows:** Creating an Azure Storage Account, enabling static website hosting, uploading HTML files, and accessing the live endpoint.

---

## Objective
Deploy and host a static HTML website using Azure Blob Storage without provisioning a traditional web server.

---

## Skills Practiced
- Creating and configuring Azure resources  
- Deploying and managing Azure Storage Accounts  
- Enabling static website hosting in Azure  
- Uploading files to Blob Storage  
- Working with storage endpoints and URLs  
- Troubleshooting web hosting errors  

---

## Tools Used
- Microsoft Azure Portal  
- Azure Storage Account  
- Azure Blob Storage  
- Static Website Hosting (Azure feature)  
- Web browser for endpoint testing  
- HTML file (example: `index.html`, `404.html`)  

---

## Steps Performed

## Hosting a Static Website on Azure

### Objective

This SOP outlines the steps to host a static website using Azure's Blob Storage service.

### Key Steps

**Step 1: Create a Resource** [0:13](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=13)

![image alt](

- Log in to your Azure account.
- Navigate to the 'Create a resource' section.
- Select 'Storage account' to create a new storage account.

**Step 2: Configure Storage Account** [0:40](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=40)


- Name your storage account (ensure it is unique).
- Select the region closest to your location (e.g., East Coast).
- Keep the preferred storage type as 'Standard'.
- Leave all other settings as default and click 'Review + create'.

**Step 3: Create the Storage Account** [1:41](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=101)


- Click 'Create' to deploy the storage account.
- Wait for the deployment to complete.

**Step 4: Enable Static Website Hosting** [2:30](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=150)


- Go to 'Data Management' in your storage account.
- Select 'Static Website'.
- Enable static website hosting.

**Step 5: Configure Index and Error Documents** [3:00](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=180)


- Set the index document name to 'index.html'.
- Set the error document name to '404.html'.
- Click 'Save'.

**Step 6: Upload Website Files** [4:40](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=280)


- Go to 'Blob service' in your storage account.
- Click on 'Web' to access the web container.
- Click 'Upload' to upload your HTML files.

**Step 7: Access Your Website** [7:04](https://loom.com/share/95c44fe345c64003a5e720a0336ec0ba?t=424)


- Copy the primary endpoint URL from the 'Static Website' section.
- Paste the URL into your web browser to access your static website.

### Cautionary Notes

- Ensure that your storage account name is unique across Azure.
- Make sure to upload the correct HTML files to the web container to avoid 'web content not found' errors.

### Tips for Efficiency

- Use a text editor like VSCode to create and edit your HTML files before uploading.
- Keep your files organized in a local directory to streamline the upload process.

---

## Outcome
Successfully hosted and accessed a static HTML website using Azure Blob Storage without deploying a dedicated web server.
