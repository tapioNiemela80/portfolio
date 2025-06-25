# Domain-Driven Design Portfolio

Tämä portfolio sisältää saman liiketoimintamallin (projektit, tiimit, jäsenet) kolmeen eri tekniseen stackiin toteutettuna, painopisteenä Domain-Driven Design (DDD), Clean Architecture ja eri tekniset toteutusmallit.

## Tavoitteet

Tarkoituksena ei ole rakentaa täydellistä liiketoimintasovellusta, vaan demonstroida:

- DDD-käsitteiden hallintaa: aggregaatit, value objectit, domain eventit
- Clean Architecturen soveltamista
- Eri teknologioiden vertailua samassa kontekstissa

## Toteutukset

| Toteutus                    | Stack | Kuvaus |
|----------------------------|-------|--------|
| [Spring Data JDBC](https://github.com/tapioNiemela80/demo-project-spring-data-jdbc) | Imperatiivinen | Kevyt ja selkeä toteutus JDBC:n päälle |
| [Reactive stack](https://github.com/tapioNiemela80/demo-project-reactive)     | Reaktiivinen WebFlux | Asynkroninen, tapahtumapohjainen malli, clean architecture |
| [Axon + Saga](https://github.com/tapioNiemela80/demo-project-axon-es)            | Event Sourcing, CQRS | Kehittyneempi malli, inter-aggregate logiikka |

### Erityishuomio Spring Data JDBC ja Reactive stack toteutuksista
- Pienillä muutoksilla sama "puhdas domain-malli" olisi käytettävissä molemmissa

##  Liiketoimintamalli
- Kaikki toteutukset noudattavat samaa liiketoimintamallia, jossa projektit koostuvat tehtävistä ja tiimit vastaavat niiden toteutuksesta.
- **Projektit**: koostuvat tehtävistä (taskeista)
- **Tiimit**: sisältävät jäseniä ja tehtäviä
- **Eventit**: kaikki mallit käyttävät domain eventtejä, joilla kommunikoidaan tilamuutoksista

## ❗ Huomio

Toteutuksessa on **tarkoituksella valittu hieman keinotekoinen liiketoimintamalli**, jonka tehtävä on antaa sopivan rikas konteksti DDD-rakenteiden esittelemiseen.

> Tarkoituksena on demonstroida teknistä osaamista, ei täysin realistista liiketoimintaa.

