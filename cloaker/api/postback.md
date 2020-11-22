---
description: "Fire conversion data to Cloakone \U0001F973"
---

# ⚓️ postback

{% api-method method="get" host="https://postback.cloakone.com" path="?clickid=XXX&value=0" %}
{% api-method-summary %}
 Postback by default
{% endapi-method-summary %}

{% api-method-description %}
​pass clickid and value in the url
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="clickid" type="string" required=false %}
clickid of visitor 
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="number" required=false %}
payout value
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
OK {"clickid":"XXX","value":"01"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://yourdomain.com/postback" path="" %}
{% api-method-summary %}
Postback with custom domain
{% endapi-method-summary %}

{% api-method-description %}
POST request only. Use any domains with cloakone api connected \( DNS installation \)
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="clickid" type="string" required=false %}
clickid of the visitor
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="number" required=false %}
payout value
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
OK {"clickid":"XXX","value":"01"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}





