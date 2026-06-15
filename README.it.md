<p align="center">
  <a href="README.md">
    <img src="https://img.shields.io/badge/language-English-blue.svg" alt="English">
  </a>
  <a href="README.it.md">
    <img src="https://img.shields.io/badge/lingua-Italiano-green.svg" alt="Italiano">
  </a>
</p>

<h1 align="center">Prenvia.me</h1>

<p align="center">
  <strong>SaaS Multi-Tenant per la Gestione delle Prenotazioni</strong>
</p>

<p align="center">
  Piattaforma di prenotazione online per professionisti e attività che operano su appuntamento.
</p>

<p align="center">
  🌐 <a href="https://prenvia.me">Piattaforma Online</a> •
  🚀 Sviluppata da zero •
  🔒 Architettura Multi-Tenant •
  💳 Integrazione Stripe
</p>

<p align="center">
  ⚠️ Attualmente disponibile in Accesso Anticipato
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Angular-20-DD0031?logo=angular&logoColor=white" alt="Angular">
  <img src="https://img.shields.io/badge/Spring_Boot-3-6DB33F?logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/Java-21-ED8B00?logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/MySQL-8-4479A1?logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/Stripe-Integrated-635BFF?logo=stripe&logoColor=white" alt="Stripe">
</p>

---

## Screenshots

<p align="center">
  <img src="docs/screenshots/homepage.png" width="30%" />
  <img src="docs/screenshots/dashboard.png" width="30%" />
  <img src="docs/screenshots/booking-page.png" width="30%" />
</p>

---

## Nota sul Repository

Questo repository pubblico non contiene il codice sorgente di Prenvia.me.

L'applicazione completa viene sviluppata e mantenuta attivamente all'interno di repository privati.

Questo repository è pubblicato esclusivamente come vetrina del progetto e contiene documentazione, screenshot e informazioni tecniche di alto livello sulla piattaforma.

---

## Panoramica

Prenvia.me è una piattaforma progettata per aiutare le attività che lavorano su appuntamento a gestire prenotazioni, servizi, disponibilità del personale e appuntamenti dei clienti attraverso un'esperienza web moderna.

Prenvia.me è nato come una sfida ingegneristica personale, sviluppata al di fuori del mio lavoro a tempo pieno come Java Developer.

Volevo costruire qualcosa che mi permettesse di andare oltre le attività quotidiane di sviluppo e di vivere l'intero ciclo di vita di un prodotto: dall'idea iniziale alla progettazione dell'architettura, dalla definizione della business logic alla modellazione del database, fino allo sviluppo frontend, al deployment e alla gestione dell'infrastruttura.

Prima di scrivere una sola riga di codice, ho dedicato tempo alla definizione dei flussi operativi, dei ruoli utente, dei permessi, delle regole di prenotazione, dei modelli di abbonamento e dell'architettura complessiva del sistema. L'obiettivo non è mai stato creare un semplice prototipo, ma costruire una piattaforma SaaS pronta per la produzione e fondata su basi solide.

Quello che era iniziato come un progetto di apprendimento si è progressivamente trasformato in qualcosa di molto più ambizioso. Con la crescita della piattaforma, ho capito che aveva un reale potenziale commerciale e ho deciso di trasformarla in un prodotto concreto.

Oggi Prenvia.me rappresenta sia il mio percorso come software engineer sia la mia ambizione di creare prodotti digitali in grado di risolvere problemi reali per le aziende.

---

## Funzionalità Principali

* Prenotazione appuntamenti online
* Architettura multi-tenant
* Pagine pubbliche di prenotazione
* Gestione del personale e delle disponibilità
* Gestione dei servizi
* Flussi di approvazione delle prenotazioni
* Gestione degli abbonamenti tramite Stripe
* Design responsive
* Internazionalizzazione (IT, EN, DE, FR, ES)
* Autenticazione e autorizzazione sicure
* Controllo degli accessi basato sui ruoli
* Personalizzazione e branding dell'attività
* Gestione dei clienti
* Notifiche e promemoria via email

---

## Stack Tecnologico

### Frontend

* Angular 20
* Angular Material
* TypeScript
* Tailwind CSS
* RxJS

### Backend

* Java 21
* Spring Boot
* Spring Security
* Spring Data JPA
* Hibernate
* REST API
* Autenticazione JWT

### Database

* MySQL

### Infrastruttura

* Docker
* Coolify
* Hetzner Cloud
* Cloudflare

### Integrazioni e Servizi

* Stripe
* Firebase Storage
* GeoNames
* Servizi Email

---

## Architettura

```text
Customer / Business Owner
            │
            ▼
     Angular Frontend
            │
            ▼
     Spring Boot API
            │
            ▼
          MySQL
            │
            ├── Stripe Billing
            ├── Firebase Storage
            ├── Email Services
            └── GeoNames Integration
```

### Architettura del Database

Il diagramma seguente illustra il modello di dominio principale e le relazioni che supportano l'architettura multi-tenant di Prenvia.me.

<p align="center"> <img src="docs/screenshots/database-architecture.png" width="90%" alt="Database Architecture"> </p>

Prenvia.me adotta un'architettura SaaS multi-tenant in cui ogni attività opera all'interno di un ambiente logicamente isolato.

Ogni tenant mantiene in modo indipendente:

* Servizi
* Membri dello staff
* Clienti
* Impostazioni dell'attività
* Disponibilità
* Prenotazioni

La piattaforma implementa inoltre il controllo degli accessi basato sui ruoli, la gestione del ciclo di vita degli abbonamenti, meccanismi di autenticazione sicuri e integrazioni con servizi esterni, garantendo al tempo stesso l'isolamento logico dei dati tra i diversi tenant.

---

## Percorso di Sviluppo

Il progetto è stato sviluppato attraverso diverse fasi:

1. Ideazione del prodotto e analisi di business
2. Progettazione dell'architettura e modellazione del dominio
3. UI/UX design e definizione dei flussi utente
4. Sviluppo backend con Spring Boot
5. Sviluppo frontend con Angular
6. Implementazione dell'architettura multi-tenant
7. Integrazione degli abbonamenti con Stripe
8. Infrastruttura, deployment e sicurezza
9. Test continui e miglioramento progressivo

---

## Perché Questo Progetto È Importante

Prenvia.me rappresenta un percorso pratico di crescita ingegneristica.

Il progetto è stato progettato, architettato e sviluppato come una sfida concreta per approfondire la mia comprensione dell'architettura software, della scalabilità, della sicurezza, dei modelli di business SaaS e dello sviluppo di prodotti digitali.

Ogni funzionalità, flusso operativo e decisione tecnica è diventata un'opportunità per imparare, migliorare e acquisire esperienza reale al di là delle attività quotidiane del mio lavoro.

Più che una semplice piattaforma di prenotazione, Prenvia è il progetto attraverso il quale continuo a crescere come ingegnere, fondatore e costruttore di prodotti digitali.

---

## Stato Attuale

Prenvia.me è attualmente disponibile in accesso anticipato.

👉 https://prenvia.me

La piattaforma è pienamente operativa e tutte le funzionalità principali sono state implementate, testate e validate.

In questa fase, l'unico elemento ancora in completamento prima del lancio commerciale ufficiale riguarda il workflow di fatturazione e gestione degli adempimenti necessari per supportare i clienti paganti.

Parallelamente, sto completando l'ecosistema che accompagnerà il lancio pubblico della piattaforma, inclusi il mio portfolio personale e la presenza online dell'attività.

Una volta completati questi ultimi passaggi, Prenvia.me passerà dall'accesso anticipato al lancio pubblico ufficiale.

Quello che è iniziato come una sfida personale di ingegneria software si è trasformato in un vero prodotto SaaS, ormai vicino agli ultimi passi prima della disponibilità commerciale.

---

## Autore

**Diego Mezzo**

Full Stack Software Engineer
Founder di Prenvia.me

📧 [dev@diegomezzo.com](mailto:dev@diegomezzo.com)

💼 https://www.linkedin.com/in/diego-mezzo-748094270
