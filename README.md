# Hikvision NVR Collection 

## Postman

Postman collection to interact with a Hikvision NVR device.

### Environment variables

In order to use this collection in Postman, you will need to set a few environment variables for both already created environments: LAN and WAN

- NVR_USERNAME
- NVR_PASSWORD
- NVR_PROTOCOL
- NVR_HOSTNAME
- NVR_PORT

#### Example:

- NVR_USERNAME=admin
- NVR_PASSWORD=mypassword
- NVR_PROTOCOL=http
- NVR_HOSTNAME=192.168.1.156
- NVR_PORT=80

For NVR_HOSTNAME, you can use either an IPv4 address (e.g., `192.168.1.156`) or a fully qualified domain name (FQDN), such as `nvr.example.com`

### Source

All the information was obtained from each PDF file available in [NVR API documentation files](./NVR%20API%20documentation%20files/)