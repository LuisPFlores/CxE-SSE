## Permissions
Administrators who interact with Global Secure Access preview features must have the Global Secure Access Administrator and Application Administrator role. 
Universal tenant restrictions require Conditional Access Administrator or Security Administrator to create and interact with Conditional Access policies and named locations.
Some features may also require other roles. See Get started with Global Secure Access for more information.

## Before you begin
To successfully deploy and test Microsoft Security Service Edge, you need the following:
1)	Entra ID Tenant with Microsoft Entra ID Premium P1 license. If needed, you can purchase licenses or get trial licenses
2)	One user with at least Global Secure Access Administrator Role and Application Administrator to configure Microsoft Security Service Edge features. 
3)	At least one user or group to function as the client test user in your tenant.
4)	One test user in a foreign tenant (to test tenant restrictions)
   
One Windows server to function as the Application server:
* Windows Server 2012 R2 or later
* Network connectivity to Entra ID Service
* Ports 80 and 443 are open to outbound traffic
* Allow access to required URLs
* One test application hosted on the application server (RDP access to a file share is used for the purpose of this document)

One Windows server to function as the Connector server:
* Windows Server 2012 R2 or later
* Network connectivity to Entra ID Service
* Confirm that you can access your test application on the application server (successful RDP connection if you are testing file share access)
* Connector server and Application server have network connectivity between them

One Windows client device
* Windows 10/11 64-bit version
* Microsoft Entra ID joined or hybrid joined
* Internet connected and no corpnet access\VPN
* Download and install the GSA agent on the client device. See The Global Secure Access Client for Windows (preview) | Microsoft Learn for details.

