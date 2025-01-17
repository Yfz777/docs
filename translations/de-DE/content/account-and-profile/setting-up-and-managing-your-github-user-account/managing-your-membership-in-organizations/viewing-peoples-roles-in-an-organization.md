---
title: Rollen von Personen in einer Organisation anzeigen
intro: You can view a list of the people in your organization and filter by their role. For more information on organization roles, see "[Roles in an organization](/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization)."
permissions: Organization members can see people's roles in the organization.
redirect_from:
- /articles/viewing-people-s-roles-in-an-organization
- /articles/viewing-peoples-roles-in-an-organization
- /github/setting-up-and-managing-your-github-user-account/viewing-peoples-roles-in-an-organization
- /github/setting-up-and-managing-your-github-user-account/managing-your-membership-in-organizations/viewing-peoples-roles-in-an-organization
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
- Accounts
shortTitle: View people in an organization
ms.openlocfilehash: d492821546b16a7c863d96867ef431362e7056ce
ms.sourcegitcommit: 67064b14c9d4d18819db8f6398358b77a1c8002a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/17/2022
ms.locfileid: "145088748"
---
## <a name="view-organization-roles"></a>Anzeigen von Organisationsrollen

{% data reusables.profile.access_org %} {% data reusables.user-settings.access_org %} {% data reusables.organizations.people %}
4. Es wird eine Liste der Personen in deiner Organisation angezeigt. Wenn du die Liste nach Rollen filtern möchtest, klicke auf **Rolle**, und wähle die gesuchte Rolle aus.
  ![Auswahl der Rolle per Klick](/assets/images/help/organizations/view-list-of-people-in-org-by-role.png)

{% ifversion fpt %}

Wenn deine Organisation {% data variables.product.prodname_ghe_cloud %} nutzt, kannst du auch die Unternehmensbesitzer*innen anzeigen, die Abrechnungseinstellungen und Richtlinien für alle Organisationen deines Unternehmens verwalten. Weitere Informationen findest du unter [Dokumentation zu {% data variables.product.prodname_ghe_cloud %}](/enterprise-cloud@latest/account-and-profile/setting-up-and-managing-your-github-user-account/managing-your-membership-in-organizations/viewing-peoples-roles-in-an-organization#view-enterprise-owners-and-their-roles-in-an-organization).

{% endif %}

{% if enterprise-owners-visible-for-org-members %}
## <a name="view-enterprise-owners-and-their-roles-in-an-organization"></a>Anzeigen von Unternehmensbesitzer*innen und deren Rollen in einer Organisation

Wenn deine Organisation über ein Unternehmenskonto verwaltet wird, kannst du die Unternehmensbesitzer*innen anzeigen, die die Abrechnungseinstellungen und Richtlinien für alle Organisationen deines Unternehmens verwalten. Weitere Informationen zu Unternehmenskonten findest du unter [Arten von {% data variables.product.prodname_dotcom %}-Konten](/get-started/learning-about-github/types-of-github-accounts).

Du kannst auch anzeigen, ob ein*e Unternehmensbesitzer*in eine bestimme Rolle in der Organisation innehat. Unternehmensbesitzer*innen können auch Organisationsmitglieder sein, eine andere Organisationsrolle innehaben oder von der Organisation unabhängig sein.

{% note %}

**Hinweis:** Wenn du ein*e Organisationsbesitzer*in bist, kannst du auch Unternehmensbesitzer*innen dazu einladen, eine Rolle in der Organisation zu übernehmen. Wenn ein*e Unternehmensbesitzer*in die Einladung annimmt, wird ein Sitz oder eine Lizenz in der Organisation aus den verfügbaren Lizenzen deines Unternehmens verwendet. Weitere Informationen zur Funktionsweise von Lizenzierungen findest du unter [Rollen in einem Unternehmen](/admin/user-management/managing-users-in-your-enterprise/roles-in-an-enterprise#enterprise-owner).

{% endnote %}

| **Unternehmensrolle** | **Organisationsrolle** | **Zugriff auf die Organisation und Auswirkungen** |
|----|----|----|----|
| Enterprise-Inhaber | Unabhängig oder keine offizielle Organisationsrolle | Diese Rolle kann nicht auf Inhalte oder Repositorys der Organisation zugreifen, verwaltet jedoch Unternehmenseinstellungen und Richtlinien, die sich auf deine Organisation auswirken. |
| Enterprise-Inhaber | Besitzer der Organisation | Diese Rolle kann Organisationseinstellungen konfigurieren und den Zugriff auf die Ressourcen der Organisation durch Teams usw. verwalten. | 
| Enterprise-Inhaber | Organisationsmitglied | Diese Rolle kann auf Ressourcen und Inhalte der Organisation (z. B. Repositorys) zugreifen, hat jedoch keinen Zugriff auf die Einstellungen der Organisation. |

Informationen zum Anzeigen aller Rollen in einer Organisation findest du unter [Rollen in einer Organisation](/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization). {% if custom-repository-roles %} Ein Organisationsmitglied kann auch über eine benutzerdefinierte Rolle für ein bestimmtes Repository verfügen. Weitere Informationen findest du unter [Verwalten benutzerdefinierter Repositoryrollen für eine Organisation](/organizations/managing-peoples-access-to-your-organization-with-roles/managing-custom-repository-roles-for-an-organization).{% endif %}

Weitere Informationen zur Rolle „Unternehmensbesitzer“ findest du unter [Rollen in einem Unternehmen](/admin/user-management/managing-users-in-your-enterprise/roles-in-an-enterprise#enterprise-owner). 

{% data reusables.profile.access_org %} {% data reusables.user-settings.access_org %} {% data reusables.organizations.people %}
4. Klicke in der linken Randleiste unter „Unternehmensberechtigungen“ auf **Unternehmensbesitzer**.
  ![Screenshot: Die Option „Unternehmensbesitzer“ im Randleistenmenü](/assets/images/help/organizations/enterprise-owners-sidebar.png)
5. Zeige die Liste der Unternehmensbesitzer*innen deines Unternehmens an. Wenn der*die Unternehmensbesitzer*in ebenfalls Mitglied deiner Organisation ist, kannst du die Rolle in der Organisation anzeigen.

  ![Screenshot: Liste der Unternehmensbesitzer*innen und deren Rolle in der Organisation](/assets/images/help/organizations/enterprise-owners-list-on-org-page.png)

{% endif %}
