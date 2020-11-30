# 🌐 Connect your domain

Once you installed your Cloakone code in a worker, attach the domain that you want to use for your campaign. First you [add a route](./#create-a-route-to-the-worker), then you [add a DNS record](./#add-a-record)

## **Create a route to the worker**

**Select your domain**, go to the **workers** section, then click **Add route**

![](../../../.gitbook/assets/cleanshot-2020-09-02-at-21.32.48-2x.png)

* Optionally, you can use a subdomain or add a custom path. 
* Then **make sure to add the  wildcard /\* at the end.** 
* your path should look any of these:

| Route | Match |
| :--- | :--- |
| domain.com/\* | cloak root domain |
| sub.domain.com/\* | cloak only subdomain |
| \*.domain.com/\* | to cloak all subdomains |
| domain.com/path\* | cloak a specific path |

* Choose the worker "cloakone", that we created previously, then click save.

![](../../../.gitbook/assets/cleanshot-2020-09-08-at-16.32.55-2x%20%281%29.png)

## Add DNS record

add a A record to your domain to the route, pointing to **192.0.2.1**

![so that cloudflare map your domain to the route we created ](../../../.gitbook/assets/cleanshot-2020-09-07-at-20.48.28-2x.png)

### Examples

{% hint style="info" %}
* with a custom path — domain.com**/safepage/\***
  * route: `domain.com/*`
  * dns record:  `@ pointing to your safe page or 192.0.2.1`
{% endhint %}

![](../../../.gitbook/assets/cleanshot-2020-11-06-at-21.23.09-2x.png)

{% hint style="info" %}
* with a subdomain
  * route: `sub.domain.com/*`
  * dns record: `sub pointing to your safe page or`

    `192.0.2.1`
{% endhint %}

![](../../../.gitbook/assets/cleanshot-2020-11-06-at-21.23.01-2x.png)

