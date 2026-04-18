# Stability Report – Podsumowanie 

Werdykt: 🟢 LOW_RISK — brak ostrzeżeń, aplikacja uznana za stabilną. 

## Rozkład elementów UI 

Łącznie przeanalizowano 1699 obiektów. Dominujące komponenty: 

- TextView — 31,96% (543 obiekty) — najczęściej występujący element 

- LinearLayout — 18,72% (318 obiektów) — główny kontener layoutu 

- Button — 16,83% (286 obiektów) — duża liczba interaktywnych elementów 

- TableRow — 3,53% (60 obiektów) 

- ImageView — 4,0% (68 obiektów) 

- FrameLayout — 2,35% (40 obiektów) 

- EditText / requestFocus — po 2,3% (39 obiektów każdy) 

- CheckBox — 1,88% (32 obiekty) 

- ScrollView — 1,71% (29 obiektów) 

Pozostałe komponenty stanowią łącznie poniżej 10% i występują sporadycznie. 

## Wnioski 

Profil UI jest typowy dla klasycznej aplikacji demonstracyjnej — szeroka różnorodność komponentów, żadnych anomalii ani podejrzanych wzorców. 
Brak ostrzeżeń sugeruje, że hierarchia widoków jest dobrze zbudowana i nie wykryto problemów z pokryciem elementów, duplikatami ID ani niestabilnymi selektorami. 

Podpisano: Mateusz Gieszczyk
Data: 28.03.2026
