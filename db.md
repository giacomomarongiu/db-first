# Descrizione 
Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

DB_NAME: car_dealer

Table name: cars

- id | INDEX |INT or BIGINT | PK | NOTNULL | UNIQUE ! AI
- vin | VARCHAR (17) | UNIQUE | NOTNULL
- type | VARCHAR (20) | NOTNULL
- brand | VARCHAR (60) | NOTNULL
- model | VARCHAR (60) | NOTNULL
- fuel | VARCHAR (30) | NOTNULL | DEFAULT('N/A')
- body_category | VARCHAR (60) | NULL | DEFAULT('N/A')
- trasmission | VARCHAR (30) | NOTNULL | DEFAULT('N/A')
- year | YEAR | NULL 
- kilometres | SMALLINT | NULL 
- color | VARCHAR (30) | NULL
- is_available | TINYINT | NOTNULL | DEFAULT(1)
- price | SMALLINT | NOTNULL
- discount | DECIMAL(4,2) | NULL
- image | VARCHAR(255) | NULL |  DEFAULT('defaultpic)
- condition | VARCHAR(50) | NOTNULL |
- description | TEXT | NULL
- position | VARCHAR(60) | NOTNULL |  DEFAULT('Updated soon')
- note | TEXT | NULL


| Nome colonna   | id             | vin            | type           | brand          | model          | fuel           | body_category  | transmission   | year    | kilometres | color         | is_available   | price  | discount | image               | condition       | description    | position                      | note   |