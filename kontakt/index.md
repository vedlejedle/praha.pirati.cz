---
layout: contacts
description: Kontakty na pražské Piráty.
keywords: kontakt, adresa, telefon, mail, facebook, kde najdu, kde jsou, pirati praha, praha
residences:
 - name: Pirátské centrum
   url: /pice
   address: |
     Na Moráni 3,
     120 00 Praha 2
   spravce: michal.jokes
   residenceImg: kontakt/novepice.jpg
   mapLink: "https://mapy.cz/zakladni?x=14.4151543&y=50.0733415&z=18&source=addr&id=9018965&q=Na%20Mor%C3%A1ni%203"
 - name: Magistrát
   url: "http://www.praha.eu/jnp/cz/o_meste/magistrat/index.html"
   address: |
     Kancelář 40, Mariánské náměstí 2, 
     110 00 Praha 1,
   spravce: jan.louzek
   residenceImg: kontakt/magistrat.jpg
   mapLink: "https://mapy.cz/zakladni?x=14.4151543&y=50.0733415&z=18&source=addr&id=9018965&q=Na%20Mor%C3%A1ni%203"
contentSize: even # zařídí že sloupce maji stejnou šířku a nikoliv 3:2 jak je default 
# Nastavení zobrazení tabulky kontaktů.
# Lze využít:
# 1) předdefinované typy (organizationEmail, organizationRedmineLink, organizationPhone, organizationTransparentAccount, organizationDataBox, piratiRootWebsite)
# 2) vlastní řádky - zde je nutné jako type dát `custom` a vyplnit `label` a `body`
contactSummaryItems:
  - type: organizationEmail
  - type: custom
    iconClass: fa fa-facebook
    label: Facebook
    body: <a href="https://www.facebook.com/CeskaPiratskaStranaPraha/">CeskaPiratskaStranaPraha</a>
  - type: custom
    iconClass: fa fa-twitter
    label: Twitter
    body: <a href="https://twitter.com/piratipraha">@piratipraha</a>
  - type: organizationRedmineLink
  - type: organizationPhone
  - type: organizationTransparentAccount
    includeMoreLink: true
  - type: organizationDataBox
  - type: piratiRootWebsite
# kontaktní osoby se nastavují v hlavičká _people
---

<div class="o-section-header o-section-header--indented">
  <h1 class="t-h2-alt">Přidejte se</h1>
</div>

Přidejte se k [pražskému sdružení](/pripoj-se) nebo k jednotlivým [místním sdružením](/mestske-casti) v [městckých částech](/mestske-casti).

<br/>

<div class="o-section-header o-section-header--indented">
  <h1 class="t-h2-alt">Představitelé</h1>
</div>
  
{% assign person = site.people | where_exp: "item","item.uid contains 'ondrej.profant'" | first  %}
{% include people/profile-badge.html item=person imgSize='big' imgStyle='round' class='c-profile-badge--centered' %}

{% assign person = site.people | where_exp: "item","item.uid contains 'adam.zabransky'" | first  %}
{% include people/profile-badge.html item=person imgSize='big' imgStyle='round' class='c-profile-badge--centered' %}


