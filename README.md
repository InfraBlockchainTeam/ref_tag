---
description: description(opt)
---

# Tags

## Tab

{% tabs %}
{% tab title="tab1" %}
tab1 content
{% endtab %}

{% tab title="tab2" %}
tab2 content
{% endtab %}
{% endtabs %}

## Hint

{% hint style="info" %}
hint text
{% endhint %}

## Card

<table data-view="cards">
<thead> <tr> <th></th> <th></th> <th></th> </tr> </thead>
<tbody>
  <tr> <td></td> <td>card1</td> <td></td> </tr>
  <tr> <td></td> <td>cards</td> <td></td> </tr>
  <tr> <td></td> <td>Card3</td> <td></td> </tr>
</tbody>
</table>

|--|---|--|
|  | 1 |  |
|  | 2 |  |
|  | 3 |  |

## Expended

<details>

<summary>title</summary>

content

</details>

## API(Swagger)

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

$$
f(x) = x * e^{2 pi i \xi x}
$$
