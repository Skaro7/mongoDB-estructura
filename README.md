# Tasca S2.03 – Estructura de dades MongoDB

## 📄 Descripció

En aquesta tasca es treballa el disseny de **bases de dades NoSQL amb MongoDB**, centrant-nos en la modelització de dades per a casos reals.  
L’objectiu és entendre com estructurar la informació utilitzant documents i col·leccions, tenint en compte les relacions entre entitats i les necessitats del negoci.

Crearem diferents bases de dades, aplicant criteris de disseny adequats a MongoDB per facilitar la consulta i manteniment de la informació.

---

## 🎯 Objectiu de la Tasca

* Dissenyar estructures de dades en MongoDB.
* Identificar entitats i relacions dins d’un domini real.
* Adaptar el model de dades al paradigma **document-oriented**.
* Facilitar l’accés eficient a la informació des del punt de vista de l’usuari final.

---

## 📋 Nivell 1 – Òptica

### Context

Una òptica anomenada **“Cul d'Ampolla”** vol informatitzar la gestió de:

* Clients/es
* Vendes d’ulleres
* Proveïdors
* Empleats/des

L’objectiu és dissenyar una base de dades MongoDB que permeti gestionar tota aquesta informació de manera eficient.

---

### 👓 Proveïdors

De cada proveïdor es vol emmagatzemar la informació següent:

* Nom
* Adreça
  * Carrer
  * Número
  * Pis
  * Porta
  * Ciutat
  * Codi postal
  * País
* Telèfon
* Fax
* NIF

Cada marca d’ulleres es compra a **un únic proveïdor**, però un proveïdor pot subministrar **diverses marques**.

---

### 🕶️ Ulleres

De cada ullera es vol saber:

* Marca
* Graduació de cada vidre
* Tipus de muntura
  * Flotant
  * Pasta
  * Metàl·lica
* Color de la muntura
* Color de cada vidre
* Preu

---

### 👤 Clients/es

De cada client/a es vol emmagatzemar:

* Nom
* Adreça postal
* Telèfon
* Correu electrònic
* Data de registre

Quan arriba un client/a nou/va, cal indicar:

* Quin client/a li ha recomanat l’establiment (si escau)

---

### 🧑‍💼 Vendes

El sistema ha d’indicar:

* Quin/a empleat/da ha venut cada ullera
* Data i hora en què s’ha realitzat la venda

---

## 🧪 Exercici 1 – Disseny de la Base de Dades

### Enunciat

Imagina que disposem d’una **interfície gràfica** des del punt de vista d’un client de l’òptica.

**Pregunta clau:**  
Com dissenyaries la base de dades en MongoDB per facilitar l’accés i gestió de tota aquesta informació?

Cal definir:

* Col·leccions necessàries
* Estructura dels documents
* Relacions entre dades (referències o documents incrustats)
* Camps clau per a consultes habituals

---

## 🧠 Conceptes Treballats

* Modelatge de dades NoSQL
* Disseny de documents MongoDB
* Relacions 1:N i N:1 en MongoDB
* Disseny orientat a consultes
* Casos d’ús reals aplicats a bases de dades

---

## 🌐 Notes Finals

Aquesta tasca és de caràcter **conceptual i de disseny**.  
No cal implementar codi, sinó justificar l’estructura de la base de dades pensant en:

* Escalabilitat
* Simplicitat
* Eficiència de consultes

MongoDB permet flexibilitat, però un bon disseny inicial és clau per a un sistema mantenible.
