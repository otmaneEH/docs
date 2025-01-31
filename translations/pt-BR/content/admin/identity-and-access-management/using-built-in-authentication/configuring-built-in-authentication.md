---
title: Configurar a autenticação integrada
intro: 'When you use the default authentication method, all authentication details are stored on {% data variables.product.product_location %}.'
permissions: 'Site administrators can configure authentication for a {% data variables.product.product_name %} instance.'
redirect_from:
  - /enterprise/admin/user-management/using-built-in-authentication
  - /enterprise/admin/authentication/using-built-in-authentication
  - /admin/authentication/using-built-in-authentication
  - /enterprise/admin/authentication/authenticating-users-for-your-github-enterprise-server-instance/using-built-in-authentication
  - /admin/identity-and-access-management/authenticating-users-for-your-github-enterprise-server-instance/using-built-in-authentication
versions:
  ghes: '*'
type: how_to
topics:
  - Accounts
  - Authentication
  - Enterprise
  - Identity
shortTitle: Configure built-in authentication
---

## About built-in authentication

By default, {% data variables.product.product_name %} uses built-in authentication. Each person creates a user account on {% data variables.product.product_location %} from an invitation or by signing up, and then authenticates with the credentials for the account to access your instance. Your {% data variables.product.product_name %} instance stores the authentication information for the account.

You can prevent unauthenticated people from creating new user accounts on your instance. For more information, see "[Disabling unauthenticated sign-ups](/admin/identity-and-access-management/using-built-in-authentication/disabling-unauthenticated-sign-ups)."

{% data reusables.enterprise_user_management.alternatively-enable-external-authentication %}

## Configurar a autenticação integrada

{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.management-console %}
{% data reusables.enterprise_management_console.authentication %}
4. Selecione **Built in authentication** (Autenticação integrada). ![Opção Select built-in authentication (Selecionar autenticação integrada)](/assets/images/enterprise/management-console/built-in-auth-select.png)

{% data reusables.enterprise_user_management.two_factor_auth_header %}
{% data reusables.enterprise_user_management.2fa_is_available %}

## Criando a sua conta

Uma vez que sua instância foi criada, você deverá criar a sua própria conta de administrador.

1. Na página "Create Admin Account" (Criar conta de administrador) em `http(s)://[hostname]/join`, defina seu nome de usuário, senha e endereço de e-mail. Em seguida, clique em **Create an account** (Criar conta). ![Criar conta de administrador](/assets/images/enterprise/site-admin-settings/create-first-admin-acct.png)
{% data reusables.enterprise_site_admin_settings.sign-in %}

## Próximas etapas

<a name="inviting-users"></a>

After you configure built-in authentication and create your administrative account, you can invite people to create accounts and use your instance. For more information, see "[Inviting people to use your instance](/admin/identity-and-access-management/using-built-in-authentication/inviting-people-to-use-your-instance)."

## Leia mais

- "[Configurar e-mail para notificações](/admin/configuration/configuring-your-enterprise/configuring-email-for-notifications)"
