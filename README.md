# Biljettpris

## Vad jag ändrade

Jag ändrade gränsen för barnpriset från 13 till 12 år. Före ändringen gav programmet en 13-åring priset 50 kr, trots att det förväntade priset var 100 kr.

## Hur jag uppdaterade testerna

De ursprungliga testerna hoppade från 10 till 20 år och missade därför felet vid 13 år. Jag lade till testfall för 12 år (50 kr), 13 år (100 kr) och 64 år (100 kr). Tillsammans med det befintliga testet för 65 år kontrollerar de nu båda sidorna av varje prisgräns.

## Hur jag kör testerna

Jag installerade Python för att kunna köra enhetstesterna i VS Code. Testerna körs med `python -m pytest -q` i terminalen.