---
layout: index
title: "Acholote"
---

# Acholote
_Acho muita coisa e tenho muitos hobbies_

<img alt="Acholote" src="acholote.jpg" style="max-width:60%;">

## Fazendo

* Lendo: [A guerra dos chips](https://www.amazon.com.br/guerra-dos-chips-batalha-tecnologia/dp/6559870936/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=1SCCH1WHAW78Z&dib=eyJ2IjoiMSJ9.VvrZUVg6rPQLlpQi4ZFA92ncOccEO_PEGSk9UGrzfngq94V-u7aCwwS3Nf1pe0-USjtMJONaBZszB0kiCuiADcZJvc7Xj2wkRoEPeLVjK9PQKkRDqJgSUTdtzuaMKBH9Mw2aO0NfewdnUhzDDvYBUCZ_i1c3X6GzzJRfip6yJA2s7mZE9LSzHNFJW_L9gX9kjxDY76rSw5bsuqL2uba0nJfA84BRC9IjEdjZfDAOy_l3U8pucuIQRHJMyeNen50a9Udc39PHMPZUQYfcT1Ns_45gG0VcD_FE8s4-1Wz9RDQ.IQSDtyDsnC_uHwOkKDZw1dz8xnyAndgjFblgrwWsaUo&dib_tag=se&keywords=chip+wars&qid=1728536853&sprefix=chip+wars%2Cspecialty-aps%2C227&sr=8-1)

## Páginas

<ul>
{% for page in site.pages %}
{% if page.title and page.url != "/" %}
     <li>
        <a href="{{ page.url }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

## Blog

<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date: "%d %b %Y" | replace: "Jan", "Jan" | replace: "Feb", "Fev" | replace: "Mar", "Mar" | replace: "Apr", "Abr" | replace: "May", "Mai" | replace: "Jun", "Jun" | replace: "Jul", "Jul" | replace: "Aug", "Ago" | replace: "Sep", "Set" | replace: "Oct", "Out" | replace: "Nov", "Nov" | replace: "Dec", "Dez" }} <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
