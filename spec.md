# Especificação Técnica - F1 Teams Hub

## Tecnologias
- HTML5
- CSS3
- JavaScript (ES6)

## Framework CSS
- Bootstrap v5.3.3

## API Externa
- Ergast API (v1)
- Base URL: https://api.jolpi.ca/ergast/f1/
- Endpoint: https://api.jolpi.ca/ergast/f1/current/driverStandings.json

---

## Modelagem de Dados

```mermaid
erDiagram
    EQUIPE ||--o{ PILOTO : possui

    EQUIPE {
        string id PK
        string nome
        string pais
        int titulos
    }

    PILOTO {
        string id PK
        string nome
        int numero
    }
