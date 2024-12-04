
# Simulare Ecosistem - OOP Laboratory 4

Acest proiect reprezintă o simulare a unui ecosistem complex în care animalele și plantele interacționează între ele. Este conceput ca un laborator pentru aprofundarea conceptelor de programare orientată pe obiecte (OOP), incluzând moștenire, polimorfism, interfețe și utilizarea unor clase abstracte.

---

## **Descrierea proiectului**

Ecosistemul simulează:
1. Creșterea și reproducerea plantelor.
2. Deplasarea și hrănirea animalelor (erbivore, carnivore, omnivore).
3. Interacțiunile dintre entitățile ecosistemului (hrănire, reproducere, eliminare la moarte).
4. Evoluția entităților în timp și evenimentele aleatorii din ecosistem.

Acest proiect încurajează utilizarea principiilor OOP prin crearea de ierarhii complexe de clase, implementarea de interfețe și scrierea unui cod modular.

---

## **Cerinte**

### 1. **Clasele principale**
- **`EntitateEcosistem` (clasă abstractă):**
  - Este baza pentru toate entitățile din ecosistem (plante și animale).
  - Atribute comune: `nume`, `energie`, `pozitie (x, y)`, `rataSupravietuire`.
  - Metode abstracte: `actioneaza()`.

- **Clase derivate:**
  - `Planta`: crește și se reproduce pe baza resurselor din ecosistem.
  - `Animal` (abstractă): include atribute specifice (`viteza`, `tipHrana`) și metode precum `mananca()`, `deplaseaza()`.
  - Subclase ale `Animal`: 
    - `Erbivor` (ex. iepure) - mănâncă plante.
    - `Carnivor` (ex. lup) - vânează alte animale.
    - `Omnivor` (ex. urs) - mănâncă atât plante, cât și animale.

### 2. **Clasa `Ecosistem`**
- Gestionează toate entitățile ecosistemului.
- Oferă funcționalități pentru:
  - Adăugarea și eliminarea entităților.
  - Simularea interacțiunilor între entități pe o hartă de dimensiuni fixe.
  - Afișarea stării ecosistemului după fiecare pas al simulării.

### 3. **Interfața `Interactiune`**
- Asigură un comportament comun pentru:
  - `ataca(Animal prada)` - pentru carnivore.
  - `reproduce()` - pentru toate entitățile.

---

## **Funcționalități suplimentare**
- **Simulare extinsă:** 
  - Timpul evoluează, iar entitățile consumă resurse, se reproduc și evoluează.
- **Evenimente aleatorii:** 
  - Furtuni, secetă, sau apariția unor noi specii.
- **Raport final:** 
  - După finalizarea simulării, ecosistemul generează un raport cu populațiile rămase și interacțiunile observate.
  
---

## **Taskuri obligatorii**

1. **Implementarea codului:**
   - Toate clasele, metodele și funcționalitățile descrise în secțiunile anterioare trebuie implementate corect.

2. **Testarea codului:**
   - Creează mai multe scenarii de testare pentru a verifica corectitudinea interacțiunilor dintre entități (ex.: un lup vânează un iepure, plantele cresc și se reproduc).

3. **Documentația proiectului:**
   - Este necesar ca fiecare student să livreze o **documentație completă** a proiectului care să includă:
     - **Descrierea claselor și ierarhiilor.**
     - **Explicația fiecărei metode.**
     - **UML diagram al proiectului.**
     - **Scenarii de utilizare (exemple concrete de rulare a simulării).**
     - **Dificultățile întâlnite și soluțiile adoptate.**

---

## **Cerințe tehnice**
- Limbaje recomandate: **Java**, **Python**, **C#**.
- Se va evalua utilizarea corectă a conceptelor OOP:
  - Moștenire.
  - Polimorfism.
  - Suprascriere și supraîncărcare.
  - Interfețe.

---

## **Punctaj**
- Implementarea completă și corectă a cerințelor de bază: **60%**.
- Funcționalități suplimentare implementate corect: **20%**.
- Documentația și claritatea codului: **20%**.

