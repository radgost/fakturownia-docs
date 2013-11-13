[Fakturownia.pl](http://fakturownia.pl/) - faktury online
===========

Szablony faktur
---------------

Korzystając z naszego systemu do fakturownia, masz dostęp do 3 wzorów faktur. Jeśli któryś z nich nie spełnia twoich oczekiwań możesz 
przygotować własny szablon. Wystarczy zalogować się do swojego konta (jeśli go jeszcze nie masz to
[tu możesz założyć darmowe konto](https://app.fakturownia.pl/signup) ) i wejść w ustawienia >>> ustawienia konta >>> szablon faktury. Następnie kliknij "dodaj nowy szablon" i otworzy się okno do edycji kodu, dzięki któremu możesz przygotować indywidualny szablon.



Przykładowe szablony Faktur:

HTML: https://github.com/radgost/fakturownia/blob/master/snieg.hbs.html

CSS: https://github.com/radgost/fakturownia/blob/master/snieg.css

Szablony są tworzone przy wykorzystaniu znaczników  [Handlebars](http://handlebarsjs.com/)

Zmienne których można używać w szablonach:

```shell
{{document_type}}
{{kind}} - typ
{{number}} - numer
{{title}} - tytuł
{{issue_date}} - data wystawienia
{{issue_place}}
{{print_option}}
{{sell_date}} - data sprzedaży
{{company}}
{{post_code}}
{{place}} - miejsce wystawienia
{{street}}
{{tax_no}} - nip
{{country}}
{{www}}
{{email}}
{{fax}}
{{phone}}
{{bank}}
{{person}}
{{bank_account}}
{{buyer}} - nabywca
{{buyer_post_code}} - kod pocztowy
{{buyer_place}}
{{buyer_street}} - ulica i nr
{{buyer_country}} - kraj
{{buyer_tax_no}} - nip
{{buyer_person}} - imię i nazwisko odbiorcy
{{buyer_company}}
{{total_price_net}} - wartość netto
{{total_price_net_with_currency}}
{{total_price_gross}} - wartość brutto
{{total_price_gross_with_currency}}
{{tax_value}}
{{tax_value_with_currency}}
{{notes}}
{{outstanding}}
{{outstanding_in_words}}
{{all_in_words}}
{{payment_to}} - termin płatności
{{type_of_payment}}
{{paid}} - kwota opłacona
{{logo_url}}
{{stamp_url}}
{{token}}
{{oid}} - nr zamówienia
{{description_long}} - dodatkowe uwagi (drukowane na drugiej stronie)
{{description_footer}} - dodatkowe uwagi (drukowane na dole strony)
{{view_url}}
{{payment_url}}
{{tax_name}}
{{currency}} - waluta
{{currency_symbol}}
{{currency_short}}
{{exchange_currency}} - przeliczanie na walutę
{{use_delivery_address}} - inny adres korespondencyjny
{{delivery_address}} - adresat
{{lang}} - język
{{discount}} - rabat
{{show_discount}}
{{income}} - przychód
{{exchange_rate}} - kurs
{{total_price_net_in_main_currency}}
{{total_price_gross_in_main_currency}}
{{additional_info}}
{{department}} - dział / oddział firmy

{{#each positions}} : 
  {{no}}
  {{item}} - nazwa produktu/usługi
  {{additional_info}} - dodatkowe pole na pozycjach faktury
  {{discount}}
  {{quantity}} - ilość
  {{unit_price_net}}
  {{unit_price_net_with_discount}}
  {{unit_price_gross}}
  {{total_price_net}} - wartość netto
  {{total_price_gross}} - wartość brutto
  {{tax}} - stawka vat
  {{tax_value}} - wartość vat 
{{/each}}

{{#each summary}} : 
  {{total_price_net}}
  {{total_price_gross}}
  {{tax}}
  {{tax_value}} 
{{/each}}

{{footer}}
```




Szablony e-maili
---------------
`TODO`

Import danych
---------------
`TODO`


API
---------------

Opis API znajduje się tu: [Fakturownia API](https://github.com/radgost/fakturownia-api)


