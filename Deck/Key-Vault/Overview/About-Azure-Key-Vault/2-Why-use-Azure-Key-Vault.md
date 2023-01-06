##

Why use Azure Key Vault?

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- Centralize application secrets
- Securely store secrets and keys
- Monitor access and use
- Simplified administration of application secrets
- Integrate with other Azure services

##

Centralizing storage of application secrets in Azure Key Vault allows you to control their

%

distribution

##

Key Vault greatly reduces the chances that secrets may be accidentally

%

leaked

##

When using Key Vault, application developers no longer need to store security information in their

%

application

##

Not having to store security information in applications eliminates the need to make this information part of the

%

code

##

An application may need to connect to a database. Instead of storing the connection string in the app's code, you can store it securely in

%

Key Vault

##

With Key Vault, your applications can securely access the information they need by using

%

URIs

##

URIs allow applications to retrieve specific versions of a secret. There is no need to write custom code to protect any of the secret information stored in

%

Key Vault

##

Access to a key vault requires proper authentication and authorization before a caller (user or application) can get

%

access

##

Authentication establishes the `_____` of the caller, while authorization determines the `_____` that they are allowed to perform.

%

Authentication establishes the **identity** of the caller, while authorization determines the **operations** that they are allowed to perform.

##

Authentication is done via Azure Active Directory. Authorization may be done via Azure role-based access control (Azure RBAC) or Key Vault

%

access policy

##

Azure RBAC can be used for both management of the vaults and access data stored in a vault, while key vault access policy can only be used when attempting to access data stored in a

%

vault

##

Azure Key Vaults may be either software-protected or, with the Azure Key Vault Premium tier, hardware-protected by 

%

hardware security modules (HSMs) 

##

Software-protected keys, secrets, and certificates are safeguarded by `_____`, using industry-standard algorithms and key lengths

%

Software-protected keys, secrets, and certificates are safeguarded by **Azure**, using industry-standard algorithms and key lengths

##

For situations where you require added assurance, you can import or generate keys in HSMs that never leave the HSM boundary. Azure Key Vault uses nCipher HSMs, which are Federal Information Processing Standards (FIPS) 140-2 Level 2 validated. You can use nCipher tools to move a key from your HSM to

%

Azure Key Vault

##

Azure Key Vault is designed so that Microsoft does not see or extract your

%

data

##

Once you have created a couple of Key Vaults, you will want to monitor how and when your keys and secrets are being accessed. You can monitor activity by enabling logging for your vaults. You can configure Azure Key Vault to:

- `_____`
- `_____`
- `_____`

%

- Archive to a storage account
- Stream to an event hub
- Send the logs to Azure Monitor logs

##

You have control over your logs and you may secure them by restricting access and you may also delete logs that you no longer

%

need

##

When storing valuable data, you must take several steps. Security information must be secured, it must follow a life cycle, and it must be highly available. Azure Key Vault simplifies the process of meeting these requirements by:

- Removing the need for in-house knowledge of `_____`.
- Scaling up on short notice to meet your organization's usage `_____`.
- Replicating the contents of your Key Vault within a region and to a secondary region. Data replication ensures high availability and takes away the need of any action from the administrator to trigger the `_____`.
- Providing standard Azure `_____` options via the portal, Azure CLI and PowerShell.
- Automating certain tasks on `_____` that you purchase from Public CAs, such as enrollment and renewal.

%

- Removing the need for in-house knowledge of **Hardware Security Modules**.
- Scaling up on short notice to meet your organization's usage **spikes**.
- Replicating the contents of your Key Vault within a region and to a secondary region. Data replication ensures high availability and takes away the need of any action from the administrator to trigger the **failover**.
- Providing standard Azure **administration** options via the portal, Azure CLI and PowerShell.
- Automating certain tasks on **certificates** that you purchase from Public CAs, such as enrollment and renewal.

##

Azure Key Vaults allow you to segregate application secrets. Applications may access only the vault that they are allowed to access, and they can be limited to only perform specific operations. You can create an Azure Key Vault per application and restrict the secrets stored in a Key Vault to a specific application and

%

team of developers

##

Key Vault itself can integrate with storage accounts, event hubs, and log analytics.

As a secure store in Azure, Key Vault has been used to simplify scenarios like:

- Azure Disk `_____`
- The always encrypted and Transparent Data Encryption functionality in `_____` server and Azure `_____` Database
- Azure `_____` Service

%

- Azure Disk **Encryption**
- The always encrypted and Transparent Data Encryption functionality in **SQL** server and Azure **SQL** Database
- Azure **App** Service
