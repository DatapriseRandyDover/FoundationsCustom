# CustomFoundations-2

These are JSON templates for a new azure foundations deployment.  The deployments include the basic infrastructure for each subscription.  They include objects like VNETs, NSGs, Virtual Network Gateways, Recovey Services Vaults, and a single Log Analytics account.

If the following templates are deployed as is they will deploy a /20 for all subscriptions and deployments.  You can change the IP ranges for any or all deployments.  The table below shows the current breakdown for each deployment. 

| IP Range |	/20 for all deployments |	NSGs |	10.0.0.0-10.0.15.255 |
| -------- | ------------------------ | ---- | --------------------- |
| Vnet_3Subnet |	/22 | |		10.0.4.0/22 |
| /24 |	AppSubnet |	NSG_App |	10.0.4.0/24 |
| /24 |	WebSubnet |	NSG_Web |	10.0.5.0/24 |
| /24 |	DBSubnet |	NSG_DB |	10.0.6.0/24 |
| Vnet_2Subnet |	/22 |		10.0.12.0/22 |
| /24 |	WVD_UsersSubnet |	NSG_Users |	10.0.12.0/24 |
| /24 |	WVD_AdminsSubnet |	NSG_Admins |	10.0.13.0/24 |
| /26 |	BastionSubnet |	None |	10.0.14.0/26 |

# 3 Subnet

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FFoundationsCustom2%2Fmain%2Fproddeploynobastion.json)


# 2 Subnet
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FFoundationsCustom2%2Fmain%2Favddeploynobastion.json)
