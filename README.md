---
description: description(opt)
---

# Tags

태그 문법 : "{&#37; 태그명 %} 내용 {&#37; end태그명 %}"


## Tab

> {&#37; tabs %}
> 
>   {&#37; tab title="tab1" %} tab1 content {&#37; endtab %}
>   
>   {&#37; tab title="tab2" %} tab2 content {&#37; endtab %}
>   
> {&#37; endtabs %}


{% tabs %}
{% tab title="tab1" %}
tab1 content
{% endtab %}

{% tab title="tab2" %}
tab2 content
{% endtab %}
{% endtabs %}

## Hint

> {&#37; hint style="info" %} hint text {&#37; endhint %}

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

> {&#37; swagger method="get" path="" baseUrl="https://test.com" summary="summary" %}
> 
> {&#37; swagger-description %} description(opt) {&#37; endswagger-description %}
> 
> {&#37; swagger-parameter in="path" name="path_param" type="string" required="false" %} desc. {&#37; endswagger-parameter %}
>
> {&#37; swagger-parameter in="query" name="query_parma" required="false" %} desc. {&#37; endswagger-parameter %}
> 
> 
> {&#37;  swagger-response status="200: OK" description="desc" %}
> 
> ```javascript
> 
> {
> 
>     // Response body
>     
> }
> 
> ```
> 
> {&#37; endswagger-response %}
> 
> {&#37; endswagger %}


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
