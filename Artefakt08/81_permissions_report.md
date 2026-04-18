# AUDYT BEZPIECZEŃSTWA: ANALIZA MANIFESTU APLIKACJI  
**Status:** Przeprowadzono automatyczną ekstrakcję potencjalnych zagrożeń.

### 1. Zawartość RiskyPermission.xml  
Wykryto następujące krytyczne wpisy:
- **Debuggable:** `true` (⚠️ WYSOKIE RYZYKO - Potencjalna podatność na ataki inżynierii wstecznej oraz analizę aplikacji).
- **Permissions:** Wykryto uprawnienia umożliwiające dostęp do lokalizacji (`ACCESS_FINE_LOCATION`) oraz odczyt i zapis do pamięci wewnętrznej.

### 2. Interpretacja Inżynierska  
Najistotniejszym zagrożeniem w kontekście bezpieczeństwa jest flaga `debuggable`, ponieważ umożliwia ona przeprowadzenie ataków związanych z debugowaniem aplikacji oraz śledzeniem jej działania przez osoby trzecie. 

### 3. Akcja korygująca  
Zaleca się implementację procesu weryfikacji w ramach pipeline CI/CD (np. Jenkins, GitLab CI), który automatycznie zablokuje tworzenie buildów w przypadku wykrycia flagi `debuggable="true"`.

####  Raport wykonanay przez:
**Podpis:** Mateusz Gieszczyk, 95009
**Data:**  18.04.2026


 