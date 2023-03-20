---
description: description(opt)
---

# Tags

태그 문법 : `{% 태그명 %}` 내용 `{ % end태그명 %}`

이하 태그블럭은 `{ 태그명 %}`로 표기함.(gitbook 표기용)

## Tab

```
 { %tabs %}
  { tab title="tab1" %} tab1 content { endtab %}
  { tab title="tab2" %} tab2 content { endtab %}
{ endtabs %}
```

{% tabs %}
{% tab title="tab1" %}
tab1 content
{% endtab %}

{% tab title="tab2" %}
tab2 content
{% endtab %}
{% endtabs %}

## Hint

```
{ hint style="info" %} hint text { endhint %}
```

{% hint style="info" %} hint text {% endhint %}

## Card

```
  <table data-view="cards">
  <thead> <tr> <th></th> <th></th> <th></th> </tr> </thead>
  <tbody>
    <tr> <td></td> <td>Card1</td> <td></td> </tr>
    <tr> <td></td> <td>Card2</td> <td></td> </tr>
    <tr> <td></td> <td>Card3</td> <td></td> </tr>
  </tbody>
  </table>
```

<table data-view="cards">
<thead> <tr> <th></th> <th></th> <th></th> </tr> </thead>
<tbody>
  <tr> <td></td> <td>Card1</td> <td></td> </tr>
  <tr> <td></td> <td>Card2</td> <td></td> </tr>
  <tr> <td></td> <td>Card3</td> <td></td> </tr>
</tbody>
</table>

## Expended

```
<details>
<summary>title</summary>
content
</details>
```

<details>
<summary>title</summary>
content
</details>

## API(Swagger)
<pre>
{ swagger method="get" path="" baseUrl="https://test.com" summary="summary" %}
{ swagger-description %} description(opt) { endswagger-description %}
{ swagger-parameter in="path" name="path_param" type="string" required="false" %} desc. { endswagger-parameter %}
{ swagger-parameter in="query" name="query_parma" required="false" %} desc. { endswagger-parameter %}

{ swagger-response status="200: OK" description="desc" %}
```javascript
{
    // Response body
}
```
{ endswagger-response %}
{ endswagger %}
</pre>

{% swagger method="get" path="" baseUrl="https://test.com" summary="summary" %}
{% swagger-description %}
description(opt)
{% endswagger-description %}

{% swagger-parameter in="path" name="path_param" type="string" required="false" %}
desc.
{% endswagger-parameter %}

{% swagger-parameter in="query" name="query_parma" required="false" %}
desc.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="desc" %}
```javascript
{
    // Response body
}
```
{% endswagger-response %}
{% endswagger %}

## Math

<pre>
$$ 
  f(x) = x * e^{2 pi i \xi x} 
$$
</pre>

$$ f(x) = x * e^{2 pi i \xi x} $$
