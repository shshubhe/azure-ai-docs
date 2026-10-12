---
author: s-polly
ms.service: azure-machine-learning
ms.topic: include
ms.date: 10/12/2026
ms.author: scottpolly
ai-usage: ai-assisted
---

> [!IMPORTANT]
> If the Azure Key Vault associated with your Azure Machine Learning workspace has public network access disabled or firewall restrictions enabled, you must enable **Allow trusted Microsoft services to bypass this firewall** on the key vault. This requirement applies even when you configure private endpoints for the key vault.
>
> Azure Machine Learning stores and retrieves workspace secrets in your key vault through its service-side infrastructure. Private endpoints in your virtual network or the workspace managed virtual network do not replace the trusted-services bypass required for this service-side access.
>
> The bypass does not grant access to every Azure service. Only eligible trusted services can use it, and requests must still authenticate with Microsoft Entra ID and have the required Azure RBAC permissions or Key Vault access-policy permissions. For more information, see [Azure Key Vault trusted services](/azure/key-vault/general/overview-vnet-service-endpoints#trusted-services).
