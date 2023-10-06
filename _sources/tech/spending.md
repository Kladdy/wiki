# Spending

Spending är ett verktyg för att hålla koll på inkomster, utgifter och innehav. Följande källor kan användas för att ladda in data till Spending:

- [Spendwise (SJ Prio Mastercard)](https://www.spendwise.se/)
- [Handelsbanken](https://www.handelsbanken.se/)
- [Swedbank](https://www.swedbank.se/)

## Konfiguration

Följande visar ett exempel av konfigurationsfilen `spending_config.yaml`:

```yaml
user: Ylva & Evert
short_user: BG1 # 2-3-letter abbreviation (e.g. Bargatan 1 -> BG1)
user_images:
- /img/1681938396974.jpeg 
- /img/proffe1-2022-crop-circle.png
sources:
- name: Everts Spendwise
  type: spendwise
  data_path: data/spendwise-evert
  settings: 
- name: Ylvas Handelsbanken
  type: handelsbanken
  data_path: data/handelsbanken-ylva
  settings:
- name: Ylvas Swedbank
  type: swedbank
  data_path: data/swedbank-ylva
  settings:
```

## Hur man hämtar data från olika källor

### Spendwise

1. Logga in i Spendwise-appen och gå till "Fakturor".
2. Förra månadens faktura finns under "Aktuell" -> "Visa fakturadetaljer" -> "Visa PDF". Tidigare fakturor finns under "Tidigare" -> *välj månad* -> "Visa PDF".
3. Dela och spara PDF:en i `data/spendwise-evert` (eller motsvarande för andra användare).

### Spendwise2

1. Gå in på [Spendwise-hemsidan](https://secure.sebkort.com/nis/m/sjse/external/t/login/index) och klicka på "Kontoutdrag".
2. Välj månad och klicka "Exportera till Excel".
3. Spara Excel-filen i `data/spendwise2-evert` (eller motsvarande för andra användare).

### Handelsbanken

1. Logga in i Handelsbankens internetbank och gå till "Konton och kort".
2. Välj det konto som du vill hämta data från.
3. Välj en period som du vill hämta data från, där perioden enbart omfattar en enskild månad.
4. Klicka på "Visa".
5. Klicka på "Exportera till Excel".
6. Spara Excel-filen i `data/handelsbanken-ylva` (eller motsvarande för andra användare).

### Swedbank

TBD
