# 👻 Shadow mode

**Shadow mode or generic mode**

By default you pass your campaign ID in your campaign Link.  If you want to hide that campaign ID from your campaign Link, you can use shadow mode

## Default mode 🔗

![](../../../.gitbook/assets/cleanshot-2020-10-24-at-16.25.11-2x.png)

This is the default mode. Notice the `CONST CAMPAIGN="*"`

In generic mode you are passing the campaign ID in your campaign URL. You can use one of these parameters to pass it.

*  utm\_campaign=XXX 
* campaign=XXX
* c=XXX

We believe that passing the campaign ID with **utm\_campaign** is safe, as most of the website are using these UTM with google analytics.

**With generic mode you can use as many campaign as your want with the same worker**

## Shadow mode 👻

There are two ways to hide your campaign ID from your campaign URL. Either use one unique url per campaign or one unique worker per campaign

### One URL per campaign

By default the cloaker recognize the campaign from the URL. You have nothing to do.

{% hint style="info" %}
It only works if you use a unique URL per campaign. \(  subdomain or path \).

example

#### with subdomain

* sub1.domain.com   ==&gt; Campaign 1
* sub2.domain.com   ==&gt; Campaign 2
* ...

#### with path

* domain.com/path1   ==&gt; Campaign 1
* domain.com/path2   ==&gt; Campaign 2
* ...
{% endhint %}

#### 

### Pass campaign ID in worker

If that doesn't work for you, another option is to pass the campaign ID in the worker code.

![](../../../.gitbook/assets/cleanshot-2020-10-24-at-16.24.59-2x.png)

 Notice the`CONST CAMPAIGN="YOUR_CAMPAIGN_ID_HERE"`

The downside is that you need to create one worker per campaign.

