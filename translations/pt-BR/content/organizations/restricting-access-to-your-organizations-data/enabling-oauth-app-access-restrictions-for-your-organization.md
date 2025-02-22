---
title: Habilitar restrições de acesso do aplicativo OAuth da sua organização
intro: Os proprietários da organização podem habilitar restrições de acesso do {% data variables.product.prodname_oauth_app %} para impedir que aplicativos não confiáveis acessem recursos da organização ao permitir que integrantes da organização usem {% data variables.product.prodname_oauth_apps %} para suas contas pessoais.
redirect_from:
- /articles/enabling-third-party-application-restrictions-for-your-organization
- /articles/enabling-oauth-app-access-restrictions-for-your-organization
- /github/setting-up-and-managing-organizations-and-teams/enabling-oauth-app-access-restrictions-for-your-organization
versions:
  fpt: '*'
  ghec: '*'
topics:
- Organizations
- Teams
shortTitle: Enable OAuth App
ms.openlocfilehash: 7ae5885530f449c8ce9981067b0d0fe8b23af0d9
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/05/2022
ms.locfileid: "145128291"
---
{% data reusables.organizations.oauth_app_restrictions_default %}

{% warning %}

**Avisos**:
- A habilitação de restrições de acesso do {% data variables.product.prodname_oauth_app %} revogará o acesso da organização para todos os {% data variables.product.prodname_oauth_apps %} e chaves SSH previamente autorizados. Para obter mais informações, confira "[Sobre as restrições de acesso do {% data variables.product.prodname_oauth_app %}](/articles/about-oauth-app-access-restrictions)".
- Depois de configurar as restrições de acesso do {% data variables.product.prodname_oauth_app %}, lembre-se de tornar a autorizar qualquer {% data variables.product.prodname_oauth_app %} que requeira acesso aos dados privados da organização continuamente. Todos os integrantes da organização precisarão criar chaves SSH, e a organização precisará criar chaves de implantação conforme necessário.
- Quando as restrições de acesso do {% data variables.product.prodname_oauth_app %} estiverem habilitadas, os aplicativos poderão usar um token OAuth para acessar informações sobre transações do {% data variables.product.prodname_marketplace %}.

{% endwarning %}

{% data reusables.profile.access_org %} {% data reusables.profile.org_settings %} {% data reusables.organizations.oauth_app_access %}
5. Em "Política de acesso a aplicativos de terceiros", clique em **Configurar restrições de acesso a aplicativos**.
  ![Botão Configurar restrições](/assets/images/help/settings/settings-third-party-set-up-restrictions.png)
6. Depois de revisar as informações sobre as restrições de acesso a terceiros, clique em **Restringir acesso a aplicativos de terceiros**.
  ![Botão Confirmação de restrição](/assets/images/help/settings/settings-third-party-restrict-confirm.png)
