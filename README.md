---
description: API calls for the user API.
---

# User\(s\)

{% api-method method="get" host="" path="/v1/users/" %}
{% api-method-summary %}
Get User\(s\)
{% endapi-method-summary %}

{% api-method-description %}
Allows you to retrieve all users
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Pagination" type="object" required=false %}
Header used to pass pagination information.  WIll default to first 10 results.
{% endapi-method-parameter %}

{% api-method-parameter name="Authentication" type="object" required=true %}
Authentication token
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Users Successfully retrieved
{% endapi-method-response-example-description %}

```
[{
  "id": 200,
  "name": "test"
},{
  "id": 201,
  "name": "other"
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="" path="/v1/users/:userId" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authentication" type="object" required=true %}
Authentication token.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="User Id" type="string" required=true %}
Id of the user you want to retrieve
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "id": 200,
  "name": "Test"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

