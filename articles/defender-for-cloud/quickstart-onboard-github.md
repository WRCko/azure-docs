---
title: 'Quickstart: Connect your GitHub repositories to Microsoft Defender for Cloud'
description: Learn how to connect your GitHub repositories to Defender for Cloud.
ms.date: 09/20/2022
ms.topic: quickstart
ms.custom: ignite-2022
---

# Quickstart: Connect your GitHub repositories to Microsoft Defender for Cloud 

With cloud workloads commonly spanning multiple cloud platforms, cloud security services must do the same. Microsoft Defender for Cloud protects workloads in Azure, Amazon Web Services (AWS), Google Cloud Platform (GCP), GitHub, and Azure DevOps (ADO).

To protect your GitHub-based resources, you can connect your GitHub organizations on the environment settings page. This page provides a simple onboarding experience (including auto discovery). 

By connecting your GitHub repositories to Defender for Cloud, you'll extend Defender for Cloud's enhanced security features to your GitHub resources. These features include:

- **Defender for Cloud's CSPM features** - Assesses your GitHub resources according to GitHub-specific security recommendations. These recommendations are also included in your secure score. Resources will be assessed for compliance with built-in standards that are specific to DevOps. Defender for Cloud's [asset inventory page](asset-inventory.md) is a multicloud enabled feature that helps you manage your GitHub resources alongside your Azure resources.

- **Microsoft Defender for DevOps** - Extends Defender for Cloud's threat detection capabilities and advanced defenses to your GitHub resources.

You can view all of the [recommendations for DevOps](recommendations-reference.md) resources.

## Prerequisites


- An Azure account with Defender for Cloud onboarded. If you don't already have an Azure account [Create an account for free](https://azure.microsoft.com/free/?WT.mc_id=A261C142F).

## Availability

| Aspect | Details |
|--|--|
| Release state: | Preview <br> The [Azure Preview Supplemental Terms](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) include other legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability. |
| Required roles and permissions: | **Contributor** on the relevant Azure subscription <br> **Security Admin Role** in Defender for Cloud <br> **GitHub Organization Administrator** |
| Clouds: | :::image type="icon" source="media/quickstart-onboard-github/check-yes.png" border="false"::: Commercial clouds <br> :::image type="icon" source="media/quickstart-onboard-github/x-no.png" border="false"::: National (Azure Government, Azure China 21Vianet) |

## Connect your GitHub account

**To connect your GitHub account to Microsoft Defender for Cloud**:

1. Sign in to the [Azure portal](https://portal.azure.com/).

1. Navigate to **Microsoft Defender for Cloud** > **Environment Settings**.

1. Select **Add environment**.

1. Select **GitHub**.

    :::image type="content" source="media/quickstart-onboard-github/select-github.png" alt-text="Screenshot that shows you where to select, to select GitHub." lightbox="media/quickstart-onboard-github/select-github.png":::

1. Enter a name, select your subscription, resource group, and region.

1. Select a **region**, **subscription**, and **resource group** from the drop-down menus.

    > [!NOTE] 
    > The subscription will be the location where Defender for DevOps will create and store the GitHub connection.

1. Select **Next: Select plans**.

1. Select **Next: Authorize connection**.

1. Select **Authorize** to grant your Azure subscription access to your GitHub repositories. Sign in, if necessary, with an account that has permissions to the repositories you want to protect

    :::image type="content" source="media/quickstart-onboard-github/authorize.png" alt-text="Screenshot that shows where the authorize button is located on the screen.":::

1. Select **Install**.

1. Select the repositories to install the GitHub application.

    > [!Note]
    > This will grant Defender for DevOps access to the selected repositories.

9.  Select **Next: Review and create**.

10. Select **Create**.

When the process completes, the GitHub connector appears on your Environment settings page.

:::image type="content" source="media/quickstart-onboard-github/github-connector.png" alt-text="Screenshot showing the Environmental page with the GitHub connector now connected." lightbox="media/quickstart-onboard-github/github-connector.png":::

The Defender for DevOps service automatically discovers the repositories you select and analyzes them for any security issues. The Inventory page populates with your selected repositories, and the Recommendations page shows any security issues related to a selected repository.

## Learn more

- You can learn more about [how Azure and GitHub integrate](https://docs.microsoft.com/azure/developer/github/).

- Learn about [security hardening practices for GitHub Actions](https://docs.github.com/actions/security-guides/security-hardening-for-github-actions).

## Next steps
Learn more about [Defender for DevOps](defender-for-devops-introduction.md).

Learn how to [configure the MSDO GitHub action](github-action.md).

Learn how to [configure pull request annotations](tutorial-enable-pull-request-annotations.md) in Defender for Cloud.
