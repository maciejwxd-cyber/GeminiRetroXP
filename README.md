# GeminiRetroXP
# 🤖 Gemini RetroXP v1.1.3 FINAL — sztuczna inteligencja Google na Windows XP!

**Natywny klient Gemini AI dla Windows XP, napisany w czystym C i Win32 API!**

Tak, dobrze czytasz! 😎 W 2026 roku można korzystać ze współczesnej sztucznej inteligencji nawet na starym Windows XP, bez instalowania przeglądarki, Pythona, .NET, Electrona czy innych ciężkich środowisk.

Program został napisany z myślą o starszych komputerach i możliwie niskim zużyciu zasobów.

**Testowany na prawdziwym Windows XP Professional SP3 32-bit.** Nie w maszynie wirtualnej!

### 💻 Co potrafi Gemini RetroXP?

- Prowadzenie rozmów z modelami Google Gemini.
- Strumieniowe wyświetlanie odpowiedzi (tekst pojawia się na bieżąco).
- Pobieranie aktualnej listy modeli dostępnych dla Twojego klucza API.
- Wysyłanie załączników, np. TXT, C, Python, JPG, PNG, PDF i innych obsługiwanych formatów.
- Analizowanie kodu źródłowego, dokumentów i obrazów.
- Zapisywanie rozmów do zwykłych plików TXT.
- Zapisywanie i wczytywanie pełnych sesji w formacie GEM wraz z kontekstem rozmowy.
- Automatyczne zapisywanie sesji.
- Odbieranie plików wygenerowanych przez model, jeśli dana funkcja jest obsługiwana przez API.
- Bezpieczne przechowywanie klucza API z wykorzystaniem Windows DPAPI.

Program korzysta bezpośrednio z Google Gemini API poprzez systemowy WinHTTP.

### ⚠️ WAŻNE — Windows XP i połączenie HTTPS!

**Jeżeli nie chcesz bawić się w dodatkowe proxy, stunnel i inne obejścia TLS, zalecam Windows XP SP3 z aktualizacjami POSReady 2009 oraz Legacy Update.**

Właśnie na tak przygotowanym Windows XP program został uruchomiony i połączył się bezpośrednio z Google Gemini API, bez żadnego zewnętrznego proxy!

**Legacy Update:** https://legacyupdate.net/

Starsze, nieaktualizowane instalacje XP mogą mieć problemy z obsługą współczesnego HTTPS, certyfikatów lub szyfrów TLS. Aktualizacje POSReady i Legacy Update są zalecaną konfiguracją, ale nie gwarantują działania bez proxy na każdej instalacji.

### 🔑 Pierwsze uruchomienie — klucz API

**Program wymaga własnego klucza Google Gemini API!**

Klucz można utworzyć w Google AI Studio:

https://aistudio.google.com/apikey

1. Uruchom `GeminiRetroXP_v1_1_3_XP.exe`.
2. Przy pierwszym uruchomieniu program poprosi o wpisanie klucza API.
3. Wklej swój klucz i zatwierdź.
4. Kliknij przycisk **„Modele API”**, aby pobrać listę modeli.
5. Wybierz dostępny model z rozwijanej listy.
6. Wpisz wiadomość w dolnym polu i kliknij **„Wyślij”**.

Gotowe! Możesz rozmawiać z Gemini na Windows XP. 😁

Klucz API jest zapisywany lokalnie i chroniony za pomocą DPAPI, dlatego nie trzeba wpisywać go ponownie przy każdym uruchomieniu. Można go zmienić przyciskiem „Klucz API...”.

**UWAGA! Po KAŻDYM uruchomieniu programu należy kliknąć przycisk „Modele API”, aby pobrać listę modeli.** Dopiero potem wybierz model, z którym chcesz rozmawiać.

### 📁 Jak działają załączniki i zapisywanie rozmów?

Przycisk **„Załącz...”** pozwala wybrać plik, który zostanie dołączony do następnej wiadomości. Można w ten sposób poprosić Gemini np. o przeanalizowanie programu napisanego w C, wyjaśnienie dokumentu albo opisanie zdjęcia.

Opcja **„Zachowaj załącznik w kontekście”** pozwala zachować załącznik w historii przekazywanej modelowi. Przy dużych plikach może to zwiększać wykorzystanie pamięci, liczbę tokenów i koszt zapytań API.

**„Zapisz”** umożliwia zapis w dwóch formatach:

**TXT** — zwykły tekst rozmowy, który otworzysz w edytorze tekstu.

**GEM** — pełna sesja programu, którą można później ponownie wczytać i kontynuować rozmowę.

Do wczytywania sesji służy przycisk **„Wczytaj”**.

### 🚀 Wymagania

**System:** Windows XP SP3 32-bit, zalecane aktualizacje POSReady 2009 i Legacy Update. Program powinien również działać na nowszych systemach Windows.

**Procesor:** kompatybilny z 32-bitowym Windows XP.

**RAM:** aplikacja podczas zwykłej rozmowy zajmowała w testach około 16 MB pamięci roboczej. Duże załączniki i długa historia zwiększają zużycie RAM.

**Internet:** wymagane działające połączenie HTTPS z Google Gemini API.

**Konto Google i własny klucz Gemini API:** wymagane. Dostępność modeli, limity i ewentualne opłaty zależą od warunków usługi Google.

### 🔧 Informacje techniczne

**Wersja:** 1.1.3 FINAL  
**Architektura:** Win32 x86 (32-bit)  
**Język programowania:** C  
**Interfejs:** Windows API / RichEdit  
**Komunikacja:** WinHTTP / HTTPS  
**Kompilator:** MinGW-w64 GCC 5.3.0  
**Zewnętrzne frameworki:** brak

Program nie zawiera wbudowanego klucza API. Każdy użytkownik musi podać własny.

To nieoficjalny, hobbystyczny klient korzystający z Google Gemini API. Nie jest produktem firmy Google.

**Mała uwaga:** nie udostępniaj nikomu swojego klucza API ani prywatnych plików sesji GEM.

---

**Stare komputery nie muszą kończyć jako elektrośmieci!** ♻️

Windows XP + czyste C + Win32 API + współczesna sztuczna inteligencja = Gemini RetroXP. 🤣

Miłego testowania!
