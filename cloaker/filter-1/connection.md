# 🌐 connection

## url [🔗](https://emojipedia.org/link/)

whitelist or blacklist url containing some param or variable 

{% hint style="info" %}
#### Example, for native source.

* you want to whitelist \( = only allow \) url containing param `sid=`
* You can whitelist widgets \#405 \#015 \#150  `405,015,150`
* or blacklist all visitors coming from widget \#450 and \#4545 `450,4545 ( widget trap )`
{% endhint %}

{% hint style="info" %}
#### Example for search

* blacklist all traffic coming from keywords "cheap", "free"  :`cheap,free`
{% endhint %}

## ip [🌐](https://emojipedia.org/globe-with-meridians/)

there are three types of IP databases.

* **global** — third parties databases. 💯
* **internal** — our private database updated in real time. 💯
* **custom** — you custom ip list 📝

#### custom list 📝

 You can set your own custom list of ip to allow / disallow

list ip \( or ip range 37.169.184.\* \) separated by comma : `37.170.*,37.169.184.233` 

{% hint style="success" %}
global and internal ip database strength are managed automatically based on the traffic score. 💯
{% endhint %}



## ISP 🏢

These are broad categories for ISP

* commercial
* organizations
* gouvernements
* education \( Universities, Schools \)
* residential
* mobile
* data center

{% hint style="success" %}
These are managed automatically based on the traffic score you set. 💯
{% endhint %}



## referer 🔙

> When visiting a web page, the _referrer_ or referring page is the URL of the previous webpage from which a link was followed. More generally, a _referrer_ is the URL of a previous item which led to this request

It's very easy to spoof the referer, and also not reliable \( referer will be blank if you go from http to https \).  
While we make this filter available, we don't recommend using it.

{% hint style="danger" %}
referer filter doesn't work in JS mode
{% endhint %}





