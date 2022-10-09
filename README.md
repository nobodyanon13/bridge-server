# bridge-server


### Setup

To setup the bridge server:
1. go to the config and edit `config.json` with this.
2. Replace the following variables in the `config.json` file with appropriate values.
    * `<SHADOWSOCKS-PASSWORD>`: A password for ShadowSocks example `!FR33DoM!`.
    * `<BRIDGE-UUID>`: The generated UUID for the bridge server example : `cfc3ac34-a70d-424e-b43c-33049cf4bf31`.
    * `<UPSTREAM-SERVER-IP>`: The upstream server IP address example `13.13.13.13`.
    * `<UPSTREAM-UUID>`: The generated UUID for the upstream server example `cfc3ac34-a70d-424e-b43c-33049cf4bf31`.
3. Run `docker-compose up -d`. 

#### UUIDs

V2Ray uses the VMESS protocol as the primary protocol.
The VMESS protocol requires UUIDs for security reasons (instead of passwords).
We need two UUIDs for the two V2Ray servers (upstream and bridge servers).

You can generate UUIDs:

1- Online:

[https://www.uuidgenerator.net](https://www.uuidgenerator.net)

Sample UUIDs:
* `cfc3ac34-a70d-424e-b43c-33049cf4bf31`
* `143d98d8-ac89-465a-acb5-d8d51e1f851f`

