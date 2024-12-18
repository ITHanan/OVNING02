
# OVNING02

# Kund- och Produktprojekt

Detta projekt innehåller SQL-frågor för att hantera och analysera data från en e-handelsdatabas. En SQL-fil finns tillgänglig i LearnPoint för att hjälpa dig att skapa databasen med data.

## Scenario
Du arbetar med en e-handelsdatabas som innehåller följande tabeller:

- **Kunder**
  - KundID
  - Namn
  - Epost
  - Stad

- **Produkter**
  - ProduktID
  - Produktnamn
  - Pris

- **Ordrar**
  - OrderID
  - KundID
  - ProduktID
  - OrderDatum

## Uppgifter
SQL-frågorna löser följande uppgifter:

1. **Hämta alla kunder från Stockholm eller Göteborg, sorterade i stigande ordning efter namn.**
2. **Hitta alla produkter som kostar mellan 100 och 500 SEK.**
3. **Hämta alla ordrar med deras kundnamn och produktnamn genom att använda JOIN.**
4. **Räkna hur många ordrar varje kund har gjort och visa endast de kunder med fler än 2 ordrar.**
5. **Visa de 5 dyraste produkterna.**

## Struktur
Projektet innehåller följande filer:

- `create_database.sql`: Skript för att skapa databasen och tabellerna samt infoga exempeldata.
- `queries.sql`: SQL-frågor som löser ovanstående uppgifter.

## Instruktioner

1. **Skapa databasen:**
   Kör `create_database.sql` för att skapa databasen och infoga data. 

   ```bash
   mysql -u [användarnamn] -p < create_database.sql
   ```

2. **Utför SQL-frågorna:**
   Kör `queries.sql` för att utföra frågorna. Du kan också kopiera och köra enskilda frågor direkt i din SQL-klient.

   ```bash
   mysql -u [användarnamn] -p < queries.sql
   ```

## Förväntade resultat

### 1. Kunder från Stockholm eller Göteborg:
En lista över kundnamn som är sorterade i stigande ordning.

### 2. Produkter mellan 100 och 500 SEK:
En lista över produkter och deras priser inom det angivna intervallet.

### 3. Ordrar med kundnamn och produktnamn:
En tabell som innehåller orderinformation, kundnamn och produktnamn.

### 4. Kunder med fler än 2 ordrar:
En lista över kunder och antalet ordrar de har gjort (endast de med fler än två).

### 5. De 5 dyraste produkterna:
En lista över produkter och deras priser, sorterade i fallande ordning efter pris.

## Krav
- MySQL eller annan kompatibel SQL-databas
- En SQL-klient för att köra skripten

## Författare
Detta projekt är skapat som en del av en utbildningsuppgift.

---


