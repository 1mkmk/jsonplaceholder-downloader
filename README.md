# jsonplaceholder-downloader

## Opis projektu
Ten projekt to aplikacja fullstack składająca się z backendu napisanego w Kotlinie oraz frontendu zbudowanego przy użyciu React. Aplikacja umożliwia przeglądanie i zarządzanie postami z zewnętrznego API.

## Struktura projektu
- `app/`: Backend w Kotlinie
- `frontend-react/`: Frontend w React
- `ansible/`: Skrypty do automatyzacji deploymentu
- `docs/`: Dokumentacja projektu

## Wymagania
- Docker i Docker Compose
- JDK 17
- Node.js 18+

## Uruchomienie projektu

### Przy użyciu Docker Compose

1. Sklonuj repozytorium:
   ```bash
   git clone [adres-repozytorium]
   ```

2. Uruchom aplikację za pomocą Docker Compose:
   ```bash
   docker compose up
   ```

   Backend będzie dostępny pod adresem: `http://localhost:8080`
   Frontend będzie dostępny pod adresem: `http://localhost:5173`

### Uruchomienie lokalnie

#### Backend (Kotlin)

1. Przejdź do katalogu backend:
   ```bash
   cd app
   ```

2. Uruchom aplikację w trybie API:
   ```bash
   ./gradlew runDevApi
   ```

   Lub w trybie CLI:
   ```bash
   ./gradlew runDevCli
   ```

#### Frontend (React)

1. Przejdź do katalogu frontend:
   ```bash
   cd frontend-react
   ```

2. Zainstaluj zależności:
   ```bash
   npm install
   ```

3. Uruchom aplikację:
   ```bash
   npm run dev
   ```

