# 📜 FixsuBot — Dziennik Zmian (Changelog)

Oficjalny rejestr aktualizacji, nowych funkcji oraz poprawek bota i dashboardu **FixsuBot**.

---

## 🚀 Aktualizacja v2.2: Dedykowane Linki Zaproszeń i Oficjalny Katalog Serwerów Premium

📅 **Data wydania:** `2026-09-05`  
🏷️ **Wydanie:** `v2-2-premium-serverlist`

Przełomowa aktualizacja dla serwerów Discord! Wprowadzamy unikalne, spersonalizowane linki zaproszeń vanity URL (fixsubot.pl/premium-serwerlist/:slug) oraz Oficjalny Publiczny Katalog Serwerów Premium z wyszukiwarką w czasie rzeczywistym i weryfikacją na poziomie konta użytkownika.

### 👑 Dedykowany Vanity URL dla Serwera (Jeden Link na Serwer)

Od teraz każdy serwer z aktywnym pakietem Premium może posiadać własny, unikalny adres URL w domenie bota. Konfiguracja odbywa się bezpośrednio w zakładce #tab-general z możliwością wyboru kanału docelowego, własnej nazwy sluga lub ID oraz generowaniem stałego kodu zaproszenia Discord.

- Własny alias URL: fixsubot.pl/premium-serwerlist/twoja-nazwa.
- Automatyczne generowanie stałych zaproszeń (bez limitu czasowego i użyć) przez bota.
- Bogata karta podglądu z metatagami OpenGraph dla czatu Discord i social media.
- Licznik unikalnych kliknięć i wejść na serwer w czasie rzeczywistym.

### 🌟 Oficjalny Publiczny Katalog Serwerów Premium

Uruchomiono prestiżowy katalog dostępny pod adresem fixsubot.pl/premium-serwerlist, prezentujący najlepsze polskie społeczności w estetyce 1:1 Cyberpunk Master Dashboard.

- Wyszukiwarka na żywo (Instant Search) filtrująca serwery, założycieli i opisy.
- Filtry sortowania: Najwięcej członków, Najpopularniejsze oraz Alfabetycznie.
- Prezentacja Założyciela serwera z odznaką korony 👑 i unikalnym tagiem.
- Interaktywne metryki online/ogółem oraz animowany equalizer ruchu.

### 👤 Weryfikacja Premium na Poziomie Użytkownika (Owner & Admin)

Uprawnienia do funkcji dedykowanego linku i katalogu serwerów przysługują, jeśli Właściciel serwera Discord lub konfigurujący Administrator posiada aktywne konto Premium. Nie musisz kupować osobnego pakietu dla serwera!

> [!WARNING]
> Gdy subskrypcja Premium wygaśnie u Właściciela i konfigurującego Administratora, serwer zostaje automatycznie i natychmiastowo wykluczony z publicznego katalogu, dbając o aktualność listy.

---

## 🚀 Aktualizacja v2.1: Wdrożenie FixsuCustomRoles

📅 **Data wydania:** `2026-08-14`  
🏷️ **Wydanie:** `v2-1-fixsucustomroles`

Wprowadzono moduł FixsuCustomRoles oraz zaawansowany silnik uprawnień bez limitów kategorii.

### 🛡️ Zaawansowany System: FixsuCustomRoles

Wprowadziliśmy nową, osobną zakładkę 'System Ról' w głównych ustawieniach. Teraz zarządzanie hierarchią, autoryzacjami oraz logiką ról jest prostsze i bardziej intuicyjne niż kiedykolwiek.

- W pełni wizualny edytor ról zintegrowany z nowym Cyberpunk UI.
- Łatwe powiązania między whitelabel botem a systemem ról Discorda.
- Automatyczne nadawanie ról (Auto-Role) w pełni konfigurowalne.

---

## 🚀 Wersja 2.0 OMEGA - Globalna Dokumentacja i Cyberpunk UI

📅 **Data wydania:** `2026-07-28`  
🏷️ **Wydanie:** `v2-0-omega`

Największa aktualizacja w historii FixsuBota. Wprowadziliśmy pełne wsparcie dla 37 języków z dynamicznym translatorem, zabezpieczenia wojskowej klasy, oraz całkowicie nowy, zjawiskowy interfejs użytkownika.

### 🌐 Globalna Dokumentacja (37 Języków)

Przebudowaliśmy cały system bazy wiedzy. Dokumentacja teraz automatycznie wykrywa Twój język i tłumaczy się w locie na jeden z 37 dostępnych wariantów. Bez bazy danych, bez lagów – wszystko natywnie w kodzie.

- Wbudowany skrypt translacyjny Google API (Zero kosztów).
- Automatyczne dopasowywanie slugów i kotwic URL.
- Natychmiastowe ładowanie strony z pominięciem Prisma DB.

### 🎨 Nowy Dashboard (Cyberpunk Aesthetic)

Stary, nudny panel to przeszłość. Wprowadziliśmy nowy motyw graficzny z elementami Glassmorphismu, neonowymi akcentami (Pink Neon) i zaawansowanymi mikro-animacjami.

- Nowe, animowane menu nawigacji z awatarami z Discorda.
- Starfield (animowane gwiazdy w tle) na wszystkich podstronach.
- Płynne przejścia i ulepszona responsywność (Mobile-first).

### 🛡️ Pancerz Klasy Wojskowej (Faza 4)

Ulepszyliśmy system obronny przed atakami. Wprowadzono nowe limity Rate Limit z zapisem w klastrach Redis.

> [!WARNING]
> Zauważysz teraz szybsze blokowanie podejrzanego ruchu HTTP. Upewnij się, że nie spamujesz API podczas tworzenia własnych integracji.

### 💎 Zmiany w Modułach Premium

Dostosowaliśmy integrację Stripe oraz tryb DEMO dla deweloperów.

```text
POST /api/premium/activate-demo
// Automatyczny Bypass dla administratorów włączony.
```

---

## 🚀 Wersja 1.9 - Moduł Ticketów i Role Reakcji

📅 **Data wydania:** `2026-07-15`  
🏷️ **Wydanie:** `v1-9-system-roles`

Wprowadzenie zaawansowanych systemów wsparcia dla społeczności Discord. Panel Ticketów oraz w pełni interaktywne role reakcyjne.

### 🎫 Zaawansowane Tickety

Możesz teraz skonfigurować do 5 różnych kategorii ticketów na swoim serwerze z unikalnymi transkryptami HTML.

- Transkrypty zapisywane automatycznie w archiwum bota.
- Możliwość przypisywania ról wsparcia do konkretnej kategorii.
- Claimowanie ticketów przez administrację (Oznaczanie jako przejęte).

### 🎭 Role Reakcyjne (Discord UI)

Dodano możliwość tworzenia ról reakcyjnych opartych na przyciskach i menu wyboru (Dropdown) z najnowszego Discord UI.

> [!WARNING]
> Stary system ról oparty na zwykłych reakcjach (emoji) został całkowicie wycofany z dniem dzisiejszym z uwagi na limity API.

---

*Więcej szczegółów na żywo: [fixsubot.pl/changelogs](https://fixsubot.pl/changelogs)*
