# MiCamino.cs

## Descripción funcional
El archivo `MiCamino.cs` contiene una representación conceptual en programación de la experiencia de una mujer en el mundo de la tecnología. Mediante clases en C# se modelan las habilidades, valores, miedos e inseguridades que enfrenta, así como su capacidad para superarlos, inspirar a nuevas generaciones y convertirse en un referente en la industria tecnológica. El archivo incluye una simulación narrativa ejecutada en el método `Main`.

---

## Descripción técnica

### Clases

#### 1. **ProfesionalTecnologia**
- **Descripción**: Clase base que modela las propiedades y acciones comunes para cualquier profesional en tecnología.

| **Propiedad**  | **Tipo**         | **Descripción**                                                                 |
|-----------------|------------------|---------------------------------------------------------------------------------|
| `Nombre`       | `string`         | Nombre del profesional en tecnología.                                          |
| `Habilidades`  | `List<string>`   | Lista de habilidades adquiridas por el profesional.                            |
| `Obstaculos`   | `List<string>`   | Lista de obstáculos enfrentados por el profesional.                            |
| `EsReferente`  | `bool`           | Indica si el profesional se considera un referente en tecnología.              |

##### Métodos
1. **`Aprender(string habilidad)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `habilidad`: (string) Habilidad adquirida por el profesional.
   - **Variables modificadas**:
     - `Habilidades` (se agrega el nuevo elemento).
   - **Condiciones/Validaciones**: No hay validaciones explícitas en el código.
   - **Descripción**: Añade la habilidad especificada a la lista de `Habilidades` y muestra un mensaje en consola indicando la nueva adquisición.
   - **Valor de retorno**: Ninguno (`void`).

2. **`EnfrentarObstaculo(string obstaculo)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `obstaculo`: (string) Obstáculo que el profesional enfrenta.
   - **Variables modificadas**:
     - `Obstaculos` (se agrega el nuevo elemento).
   - **Condiciones/Validaciones**: No hay validaciones explícitas en el código.
   - **Descripción**: Añade el obstáculo especificado a la lista de `Obstaculos` y muestra un mensaje en consola indicando el desafío enfrentado.
   - **Valor de retorno**: Ninguno (`void`).

---

#### 2. **MujerEnTecnologia**
- **Descripción**: Clase derivada de `ProfesionalTecnologia` que modela aspectos adicionales como valores, logros y generaciones impactadas.

| **Propiedad**             | **Tipo**         | **Descripción**                                              |
|---------------------------|------------------|--------------------------------------------------------------|
| `Valores`                 | `List<string>`   | Lista de valores que guían a la profesional.                 |
| `Logros`                  | `List<string>`   | Lista de logros alcanzados por la profesional.               |
| `GeneracionesImpactadas`  | `List<string>`   | Lista de generaciones que han sido inspiradas.               |

##### Métodos
1. **`MujerEnTecnologia(string nombre)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `nombre`: (string) Nombre de la mujer en tecnología.
   - **Variables modificadas**:
     - `Nombre` (asignado el parámetro recibido).
     - `EsReferente` (iniciado en `true`).
   - **Condiciones/Validaciones**: No hay validaciones explícitas en el código.
   - **Descripción**: Constructor que inicializa el objeto con el nombre proporcionado y establece que es un referente.
   - **Valor de retorno**: Ninguno (es constructor).

2. **`AbrazarValor(string valor)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `valor`: (string) Valor adoptado por la profesional.
   - **Variables modificadas**:
     - `Valores` (se agrega el nuevo valor).
   - **Descripción**: Añade el valor especificado a la lista de `Valores` y muestra un mensaje en consola indicando que vive conforme a dicho valor.
   - **Valor de retorno**: Ninguno (`void`).

3. **`Lograr(string logro)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `logro`: (string) Logro alcanzado por la profesional.
   - **Variables modificadas**:
     - `Logros` (se agrega el nuevo logro).
   - **Descripción**: Añade el logro especificado a la lista de `Logros` y muestra un mensaje en consola indicando lo alcanzado.
   - **Valor de retorno**: Ninguno (`void`).

4. **`Inspirar(string generacion)`**
   - **Lenguaje**: C#
   - **Parámetros**:
     - `generacion`: (string) Generación impactada por la profesional.
   - **Variables modificadas**:
     - `GeneracionesImpactadas` (se agrega el nuevo elemento).
   - **Descripción**: Añade la generación especificada a la lista de `GeneracionesImpactadas` y muestra un mensaje en consola indicando la inspiración generada.
   - **Valor de retorno**: Ninguno (`void`).

5. **`CompartirConocimiento()`**
   - **Lenguaje**: C#
   - **Descripción**: Muestra un mensaje en consola indicando que la profesional comparte su conocimiento para apoyar a otras mujeres en tecnología.
   - **Valor de retorno**: Ninguno (`void`).

---

#### 3. **MujerReferente**
- **Descripción**: Clase derivada de `MujerEnTecnologia` que modela experiencias específicas como miedos, inseguridades y procesos para superarlos.

| **Propiedad**      | **Tipo**         | **Descripción**                                                                 |
|--------------------|------------------|---------------------------------------------------------------------------------|
| `Miedos`           | `List<string>`   | Lista de miedos reconocidos por la profesional.                                 |
| `Inseguridades`    | `List<string>`   | Lista de inseguridades reconocidas por la profesional.                          |

##### Métodos
1. **`IncorporarseAlMundoTecnologico()`**
   - **Lenguaje**: C#
   - **Descripción**: Representa el proceso inicial de decisión para entrar al mundo de la tecnología, enfrentando la ausencia de modelos femeninos y adquirió varias habilidades (`Conocimiento STEM`, `Pensamiento crítico` y `Trabajo en equipo`).
   - **Valor de retorno**: Ninguno (`void`).

2. **`SufrirSindromeDelImpostor()`**
   - **Lenguaje**: C#
   - **Descripción**: Añade miedos e inseguridades relacionadas con el síndrome del impostor a las propiedades correspondientes y muestra mensajes en consola describiendo el proceso.
   - **Valor de retorno**: Ninguno (`void`).

3. **`EnfrentarMiedosEInseguridades()`**
   - **Lenguaje**: C#
   - **Descripción**: Enumera los miedos e inseguridades, los reconoce y los supera, concluyendo con la adopción de valores positivos y el logro de confianza propia.
   - **Valor de retorno**: Ninguno (`void`).

4. **`AlzarLaVozYSerVisible()`**
   - **Lenguaje**: C#
   - **Descripción**: Simboliza el acto de levantar la voz y convertirse en un referente, inspirando nuevas generaciones y logrando visibilidad en la industria.
   - **Valor de retorno**: Ninguno (`void`).

---

## Esquema del orden de ejecución

```text
Programa.Main()
 ├─ MujerReferente("Lucía")
 │   ├─ AbrazarValor("Pasión")
 │   ├─ AbrazarValor("Curiosidad")
 │   ├─ AbrazarValor("Empatía")
 │   ├─ IncorporarseAlMundoTecnologico()
 │   │   ├─ Aprender("Conocimiento STEM")
 │   │   ├─ Aprender("Pensamiento crítico")
 │   │   ├─ Aprender("Trabajo en equipo")
 │   ├─ SufrirSindromeDelImpostor()
 │   ├─ EnfrentarMiedosEInseguridades()
 │   │   ├─ AbrazarValor("Confianza")
 │   │   ├─ Lograr("Reconocer su propio valor")
 │   ├─ AlzarLaVozYSerVisible()
 │       ├─ CompartirConocimiento()
 │       └─ Inspirar("Nuevas generaciones de mujeres en tecnología")
 └─ Mensajes finales
```

---

## Notas adicionales
Este archivo incluye conceptos narrativos que pueden ser útiles para aplicaciones educativas, simulaciones inspiracionales o como base para videojuegos/experiencias interactivas.


SHA:936ce71e7716fa505804560622669f6957f07523