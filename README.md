<p align="center">
  <a href="https://instantcommerce.io/" target="_blank" align="center">
    <img src="https://avatars.githubusercontent.com/u/93975473?s=200" alt="Instant Commerce" width="100">
  </a>
  <h1 align="center">shopify-headless-theme</h1>
  <p align="center">
    Liquid theme that automatically redirects customers to your custom storefront.<br>
    <a href="https://github.com/instantcommerce/shopify-headless-theme/archive/refs/heads/master.zip" download>Download theme</a></p>
</p>

---

## Purpose

When using a headless Shopify setup, you normally don't want customers to access any of the theme pages except the checkout. However, you can't totally disable the theme and a lot of links will still point to the theme (e.g. links in emails, plugins and the checkout).

The sole purpose of this Liquid theme is to automatically redirect customers that land on one of the theme pages to the related page in your custom storefront.

## Installation

1. Download the [shopify-headless-theme-master.zip](https://github.com/instantcommerce/shopify-headless-theme/archive/refs/heads/master.zip) file
2. Navigate to **Online Store > Themes** in your Shopify admin
3. Upload the theme to your **Theme Library**
4. Click the **Customize** button of the newly installed theme
5. Configure the `storefront_hostname` in **Theme settings > Storefront**
6. **Publish** the theme 🚀

## Custom redirects

You can configure the `custom_redirects` value in **Theme settings > Storefront**.

The redirect rule format is as following:

```
Shopify path > Storefront path
```

Each line in the textarea represents a single redirect rule.

### Example configuration

The example below removes the `/account` prefix from the login, register and reset password redirects.

```
/account/login > /login
/account/register > /register
/account/reset > /reset-password
/account/activate > /activate-account
```

## Multipass login

Enable the `multipass_login` option in **Theme settings > Storefront** if you implemented [Multipass](https://shopify.dev/api/multipass) (a Shopify Plus feature) in your storefront. Enabling this feature will also redirect customers from the Shopify login page to your custom storefront. If not enabled, a customizable login page will be shown when customers click the "Log in" link in the checkout.

## Gift cards

Since the Shopify Storefront API unfortunately does not support fetching gift cards yet, a customizable `gift_card.liquid` template has been added.
