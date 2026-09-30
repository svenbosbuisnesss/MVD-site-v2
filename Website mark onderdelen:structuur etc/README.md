This website is in production.

## Contactformulier en SMTP

Het contactformulier stuurt aanvragen naar `contact@markvandis.nl` via SMTP. Stel deze variabelen in op de server of bij de hostingprovider; `env.example` is alleen een invultemplate en wordt niet automatisch geladen:

- `SMTP_HOST`: SMTP-hostnaam van de mailprovider
- `SMTP_PORT`: meestal `587` voor STARTTLS of `465` voor TLS
- `SMTP_SECURE`: `true` voor TLS op poort 465; anders `false`
- `SMTP_USER` en `SMTP_PASS`: SMTP-inloggegevens
- `SMTP_FROM`: optioneel afzenderadres dat door de provider is toegestaan; standaard `SMTP_USER`

Deel SMTP-wachtwoorden niet in de chat en commit ze niet naar Git. Zonder volledige SMTP-configuratie retourneert het contactendpoint een fout in plaats van een verzendbevestiging.
