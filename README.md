# Hikvision NVR Collection

Postman collection with **two environments** (LAN and WAN) to interact with a Hikvision NVR device.

## Device tested

- Brand: Hikvision
- Model: [DS-7104NI-Q1 / 4P](https://www.hikvision.com/es-la/products/IP-Products/Network-Video-Recorders/Value-Series/ds-7104ni-q1-4p/)

> [!IMPORTANT]
> If you attempt to use this collection on a different device, some HTTP requests may not function as expected. This is because each NVR device contains distinct APIs tailored to its specific use case
> 
> However, most of the general requests will likely work on your device

## 🛠️ Environment Variables

To use this collection in Postman, you need to configure the following environment variables for both environments:

- **`NVR_USERNAME`**  
- **`NVR_PASSWORD`**  
- **`NVR_PROTOCOL`**  
- **`NVR_HOSTNAME`**  
- **`NVR_PORT`**

### 🔧 Example Configuration (needed in Step 4 below)

```bash
NVR_USERNAME=admin
NVR_PASSWORD=mypassword
NVR_PROTOCOL=http
NVR_HOSTNAME=192.168.1.156
NVR_PORT=80
```

For `NVR_HOSTNAME`, you can use:

- An IPv4 address (e.g., `192.168.1.156`)
- A Fully Qualified Domain Name (FQDN) (e.g., `nvr.example.com`)

## What to do once in Postman

Complete the following steps:

1. You might want to create a separated *Workspace* to have things organized although this is an optional step
    - Choose a Blank Workspace and select Next
    - Choose a name for the new workspace and select *Only me* for who can access to it, if you prefer so. Select Create

2. Now, go to the *Import* option next to your workspace name and drop the three files available from this [repository folder](./Postman/) and *Select Import*

    #### Postman collection

    * Hikvision DS-7104NI-Q1 - 4P NVR collection.postman_collection.json

    #### Environments

    * [LAN] - Hikvision DS-7104NI-Q1 - 4P NVR.postman_environment.json
    * [WAN] - Hikvision DS-7104NI-Q1 - 4P NVR.postman_environment.json

3. Once import process is finished, you can then go to the *Collections* and *Environments* to check if it has been done correctly

4. Go to *Environments* tab and set your environments variables for both *LAN* and *WAN* environments and use the *Current value* column to fill the data
   
5. From the right top dropdown menu, select the environment you want to work with next

6. Finally, go to *Collections* tab and try your requests. Remember: Some of the requests may not work for other NVR devices

## 📂 Source

All information was obtained from the PDF files available in the [NVR API documentation files](./NVR%20API%20documentation%20files/)