---
description: how we should load your page
---

# 🔀 method

## What is it? 🤔

We have four ways to load your page :

* [redirect](method.md#redirect) 🔗
* [iframe](method.md#iframe) 🌃
* [reverse proxy](method.md#reverse-proxy) ☁️
* stay 🪑

## Recommendation

It depends of your installation JS or DNS

### FOR JS

![](../../.gitbook/assets/cleanshot-2020-11-15-at-13.49.23-2x.png)

### FOR DNS

![](../../.gitbook/assets/cleanshot-2020-11-15-at-13.49.27-2x.png)

![](../../.gitbook/assets/cleanshot-2020-08-27-at-18.15.17-2x.png)

## Reverse proxy ☁️

* The reverse proxy load your page content with no redirection

{% hint style="info" %}
With reverse proxy, you can use these special features:

* match your lander and your offer dynamically. \( name, link, images\) 
* add tracking
* fire pixel
{% endhint %}

{% hint style="warning" %}
reverse proxy is recommended method, but in some case it might not work

* if you notice the layout of the page is broken
* if you \( or the advertiser \) are using a tracker on top of cloakone, It will see the IP of one of our server, not of the original visitor IP. So the tracker geo rules will likely not work.

If reverse proxy is not possible for your use case, then use iframe for money page
{% endhint %}

## Iframe 🌃

* Load your page inside an iframe. No change in the URL, but if you inspect the page code, you will the see &lt;iframe&gt; tag. 

{% hint style="danger" %}
**Not recommended for safe page,** but is ok for money page.
{% endhint %}

## Redirect 🔗

* redirect to another page. URL will change.

{% hint style="danger" %}
**Not recommended for money page,** but is ok for safe page.
{% endhint %}

## Stay 🪑

* Will stay on the current page. Best case scenario but require you to build you safe page \( vs reverse proxy allow you to use any website as your safe page \) 

## Summing up 👉

| METHOD | money page | safe page |
| :--- | :--- | :--- |
| reverse proxy | ✅best,  recommended | ✅best, recommended |
| iframe | ✅ ok | ❌not recommended |
| redirect | ❌ not recommended | ✅ok |
| stay | - | ✅best |

