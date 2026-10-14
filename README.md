# passport-visa-data

Visa requirements for holders of each country's passport, extracted weekly from the English Wikipedia
articles "Visa requirements for X citizens" and normalized by [TravelersBook](https://travelersbook.app).

`data/passport-visa.csv`

| column | meaning |
|---|---|
| passport_country | passport holder's country (ISO 3166-1 alpha-2) |
| destination_country | destination (ISO 3166-1 alpha-2) |
| category | visa_free · visa_on_arrival · e_visa · eta · visa_required · refused · unknown |
| stay_value, stay_unit | allowed stay as written (day · week · month · year · unlimited) |
| requirement_text | the original text of the article's requirement cell |
| source_url | the Wikipedia revision the row was taken from |

Not included: Taiwanese passports (TravelersBook uses Taiwan's Bureau of Consular Affairs list instead),
Hong Kong / Macau SAR passports, and places without an ISO 3166-1 code.

**This is not legal or travel advice.** Rules change; check the destination's official source before you travel.

## License

CC BY-SA 4.0 — adapted from Wikipedia contributors' work. See [LICENSE](LICENSE).
