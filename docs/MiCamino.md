# MiCamino.cs

## 1. Nombre del archivo:
**MiCamino.cs**

## 2. Descripción funcional:
Este archivo define una jerarquía de clases relacionadas con profesionales en tecnología, centrándose especialmente en las mujeres en tecnología. Realiza un seguimiento de sus habilidades, valores, logros y obstáculos, además de permitir modelar acciones como aprender, enfrentar retos, abrazar valores, inspirar a generaciones y compartir conocimiento. También expresa las dificultades y motivaciones específicas de una mujer referente dentro del mundo tecnológico.

## 3. Descripción técnica:

### **Clases Definidas**
1. **ProfesionalTecnologia**
2. **MujerEnTecnologia** (hereda de `ProfesionalTecnologia`)
3. **MujerReferente** (hereda de `MujerEnTecnologia`)

---

### **Clase `ProfesionalTecnologia`**

#### Lenguaje:
C#

#### Propiedades:
- **`Nombre`**: (`string`) Nombre del profesional tecnológico.
- **`Habilidades`**: (`List<string>`) Lista de habilidades adquiridas.
- **`Obstaculos`**: (`List<string>`) Lista de obstáculos enfrentados.
- **`EsReferente`**: (`bool`) Indica si el profesional es un referente (protegida).

#### Métodos:

##### **Aprender**
- **Parámetros**:
  - `habilidad` (`string`): La habilidad que se aprenderá.
- **Variables modificadas**:
  - Añade `habilidad` a la lista `Habilidades`.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método permite agregar una nueva habilidad a la lista de habilidades del profesional. Además, imprime un mensaje indicando qué habilidad se aprendió.
- **Valor de retorno**:
  - Ninguno (`void`).

---

##### **EnfrentarObstaculo**
- **Parámetros**:
  - `obstaculo` (`string`): Obstáculo enfrentado.
- **Variables modificadas**:
  - Añade `obstaculo` a la lista `Obstaculos`.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método registra un obstáculo enfrentado por el profesional y muestra un mensaje descriptivo del obstáculo.
- **Valor de retorno**:
  - Ninguno (`void`).

---

### **Clase `MujerEnTecnologia`**

#### Herencia:
Hereda de la clase `ProfesionalTecnologia`.

#### Propiedades:
- **`Valores`**: (`List<string>`) Lista de valores que guían al profesional.
- **`Logros`**: (`List<string>`) Lista de logros obtenidos.
- **`GeneracionesImpactadas`**: (`List<string>`) Generaciones que han sido inspiradas por la profesional.

#### Constructores:

##### **MujerEnTecnologia**
- **Parámetros**:
  - `nombre` (`string`): Nombre de la mujer en tecnología.
- **Variables modificadas**:
  - Asigna `nombre` a la propiedad `Nombre`.
  - Establece `EsReferente` como `true`.
- **Descripción**:
  Constructor que inicializa la instancia de la clase con un nombre y establece que este profesional tecnológico es un referente.
- **Valor de retorno**:
  - Ninguno (constructor).

---

#### Métodos:

##### **AbrazarValor**
- **Parámetros**:
  - `valor` (`string`): Valor que será abrazado por la profesional.
- **Variables modificadas**:
  - Añade `valor` a la lista `Valores`.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método registra un valor importante para el profesional y genera un mensaje informativo.
- **Valor de retorno**:
  - Ninguno (`void`).

---

##### **Lograr**
- **Parámetros**:
  - `logro` (`string`): Logro obtenido por la profesional.
- **Variables modificadas**:
  - Añade `logro` a la lista `Logros`.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método registra un logro y muestra un mensaje congratulatorio.
- **Valor de retorno**:
  - Ninguno (`void`).

---

##### **Inspirar**
- **Parámetros**:
  - `generacion` (`string`): Generación inspirada por la profesional.
- **Variables modificadas**:
  - Añade `generacion` a la lista `GeneracionesImpactadas`.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método registra la generación inspirada y genera un mensaje informativo.
- **Valor de retorno**:
  - Ninguno (`void`).

---

##### **CompartirConocimiento**
- **Parámetros**:
  - Ninguno.
- **Variables modificadas**:
  - Ninguna.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método genera un mensaje indicando que la profesional está compartiendo su conocimiento para apoyar a otras mujeres en tecnología.
- **Valor de retorno**:
  - Ninguno (`void`).

---

### **Clase `MujerReferente`**

#### Herencia:
Hereda de la clase `MujerEnTecnologia`.

#### Propiedades:
- **`Miedos`**: (`List<string>`) Lista de miedos de la mujer referente.
- **`Inseguridades`**: (`List<string>`) Lista de inseguridades de la mujer referente.

#### Constructores:

##### **MujerReferente**
- **Parámetros**:
  - `nombre` (`string`): Nombre de la mujer referente.
- **Variables modificadas**:
  - Llama al constructor de la clase base para inicializar `Nombre` y `EsReferente`.
- **Descripción**:
  Constructor que inicializa la instancia con el nombre de la profesional y características propias de las mujeres referentes.
- **Valor de retorno**:
  - Ninguno (constructor).

---

#### Métodos:

##### **IncorporarseAlMundoTecnologico**
- **Parámetros**:
  - Ninguno.
- **Variables modificadas**:
  - Modifica las listas `Habilidades`, `Miedos` e `Inseguridades` de la profesional.
- **Condiciones/Validaciones**:
  - Ninguna.
- **Descripción**:
  Este método modela la entrada de la mujer referente al mundo tecnológico, agregando habilidades esenciales, además de explicar miedos e inseguridades comunes, mediante mensajes descriptivos.
- **Valor de retorno**:
  - Ninguno (`void`).

---

## 4. Esquema del orden de ejecución:

```plaintext
ProfesionalTecnologia
  ├── Aprender()
  ├── EnfrentarObstaculo()
  │
MujerEnTecnologia (hereda de ProfesionalTecnologia)
  ├── AbrazarValor()
  ├── Lograr()
  ├── Inspirar()
  ├── CompartirConocimiento()
  │
MujerReferente (hereda de MujerEnTecnologia)
  ├── IncorporarseAlMundoTecnologico()
      ├── Aprender() [llamado internamente]
      ├── Modifica:
          ├── Miedos
          ├── Inseguridades
```

## 5. Notas adicionales:
- Todas las clases son parte del espacio de nombres `W4TT`.
- Los métodos incluyen interacciones con la consola (`Console.WriteLine`) para describir simbólicamente las acciones realizadas por cada profesional.
- El diseño de las clases promueve la extensión mediante herencia para modelar diferentes tipos de profesionales en tecnología.
```markdown
# MiCamino.cs

## 1. Nombre del archivo
**MiCamino.cs**

## 2. Descripción funcional
Este archivo implementa un programa en C# cuyo objetivo es narrar simbólicamente el proceso de una mujer, "Lucía", al desenvolverse en el mundo de la tecnología. A través de diversas etapas, Lucía enfrenta inseguridades y miedos, se supera, abraza sus valores, y se convierte en un referente inspirador para futuras generaciones de mujeres en tecnología.

## 3. Descripción técnica

### 3.1. Clase `MujerReferente`
La clase `MujerReferente` representa el viaje simbólico de una mujer en el mundo tecnológico. Esta clase encapsula propiedades y métodos para gestionar las emociones, acciones, y logros de la protagonista.

#### Propiedades
- **Nombre** *(string)*  
  Almacena el nombre de la protagonista.
- **Miedos** *(List<string>)*  
  Lista que representa los miedos enfrentados por la protagonista.
- **Inseguridades** *(List<string>)*  
  Lista que representa las inseguridades internas de la protagonista.

### 3.2. Métodos

#### `AbrazarValor`
- **Lenguaje:** C#
- **Parámetros:**  
  - `valor` *(string)*: Representa el valor que la protagonista decide incorporar a sí misma.
- **Variables modificadas:**  
  No modifica propiedades a nivel interno o global.
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  Recibe un valor como argumento y muestra un mensaje en la consola afirmando que la protagonista lo adopta como parte de su camino. 
- **Valor de retorno:**  
  Ninguno.

#### `IncorporarseAlMundoTecnologico`
- **Lenguaje:** C#
- **Parámetros:**  
  Ninguno.
- **Variables modificadas:**  
  No modifica propiedades internas directamente.
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  Muestra mensajes destacando que la protagonista ha decidido entrar al mundo de tecnología, enfrentando un entorno sin referentes previos.
- **Valor de retorno:**  
  Ninguno.

#### `SufrirSindromeDelImpostor`
- **Lenguaje:** C#
- **Parámetros:**  
  Ninguno.
- **Variables modificadas:**  
  - `Miedos`: Se añaden los miedos **"Ser juzgada"** y **"No estar a la altura"**.  
  - `Inseguridades`: Se añade la inseguridad **"No soy lo suficientemente buena"**.
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  Este método simula cómo la protagonista comienza a sentir el síndrome del impostor, acumulando miedos e inseguridades que son reflejados en las listas correspondientes.
- **Valor de retorno:**  
  Ninguno.

#### `EnfrentarMiedosEInseguridades`
- **Lenguaje:** C#
- **Parámetros:**  
  Ninguno.
- **Variables modificadas:**  
  - `Miedos`: Se limpian (se eliminan todos los elementos).  
  - `Inseguridades`: Se limpian (se eliminan todos los elementos).
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  Simula el proceso de enfrentamiento de los miedos e inseguridades de la protagonista al iterar sobre ellos, mostrando en consola los mensajes correspondientes al enfrentamiento y refuerzo de autoestima. Finalmente, las listas de miedos e inseguridades se vacían y se registran valores emocionalmente positivos con el método `AbrazarValor`. Además, marca el logro de "Reconocer su propio valor".
- **Valor de retorno:**  
  Ninguno.

#### `AlzarLaVozYSerVisible`
- **Lenguaje:** C#
- **Parámetros:**  
  Ninguno.
- **Variables modificadas:**  
  No modifica propiedades internas directamente.
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  La protagonista reclama su espacio en tecnología con un mensaje visible, inspirando a nuevas generaciones y consolidando un papel destacado en el sector. Utiliza métodos auxiliares, como `CompartirConocimiento()` y `Inspirar()`, y marca un logro simbólico: "Convertirse en una voz visible en la industria".
- **Valor de retorno:**  
  Ninguno.

### 3.3. Clase `Programa`
La clase `Programa` contiene el punto de entrada de la aplicación (método `Main`).

#### Método `Main`
- **Lenguaje:** C#
- **Parámetros:**  
  - `args` *(string[])*: Argumentos de la consola (no utilizados en esta implementación).
- **Variables modificadas:**  
  Ninguna.
- **Condiciones, validaciones o requisitos:**  
  Ninguna.
- **Descripción:**  
  Crea una instancia de la clase `MujerReferente` con el nombre "Lucía" y ejecuta una serie de métodos para narrar su historia:  
  - `AbrazarValor` se utiliza para incorporar valores positivos.  
  - Se llaman los métodos `IncorporarseAlMundoTecnologico`, `SufrirSindromeDelImpostor`, `EnfrentarMiedosEInseguridades`, y `AlzarLaVozYSerVisible` en orden para estructurar los capítulos simbólicos de su trayectoria.  
  Al finalizar, imprime un mensaje motivacional que subraya la importancia de las mujeres en tecnología.
- **Valor de retorno:**  
  Ninguno.

---

## 4. Esquema del orden de ejecución

```plaintext
Main
└── MujerReferente("Lucía") <- Inicialización
    ├── AbrazarValor("Pasión")
    ├── AbrazarValor("Curiosidad")
    ├── AbrazarValor("Empatía")
    ├── IncorporarseAlMundoTecnologico()
    ├── SufrirSindromeDelImpostor()
    ├── EnfrentarMiedosEInseguridades()
    │   ├── Iteración sobre Miedos
    │   ├── Iteración sobre Inseguridades
    │   ├── AbrazarValor("Confianza")
    │   └── Lograr("Reconocer su propio valor")
    ├── AlzarLaVozYSerVisible()
    │   ├── CompartirConocimiento()
    │   ├── Inspirar("Nuevas generaciones de mujeres en tecnología")
    │   └── Lograr("Convertirse en una voz visible en la industria")
    └── Mensaje final en la consola
```

---

## 5. Comentarios finales
El archivo `MiCamino.cs` es un enfoque simbólico para ilustrar los retos y triunfos de las mujeres en tecnología. Si bien no cumple una función técnica convencional, su implementación sirve como una narrativa inspiradora programada en C#. Es un ejemplo donde el código trasciende su propósito funcional para transmitir un mensaje más profundo y humano.
```


SHA:936ce71e7716fa505804560622669f6957f07523