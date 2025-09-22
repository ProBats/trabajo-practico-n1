# 💳 Sistema Bancario - Proyecto Java

## 🧾 Descripción

Este proyecto en Java que simula un sistema bancario orientado a objetos. Permite la gestión de diferentes tipos de clientes y cuentas, con funcionalidades bancarias típicas, validaciones robustas, menús interactivos y separación por tipo de cliente (individual o empresa).

- Gestión de saldos
- Depósitos y extracciones
- Manejo de cheques
- Conversión entre pesos y dólares

---

## 🧠 Funcionalidades principales

### 👥 Tipos de clientes:
- 🧑 `ClienteIndividual`: Persona física con nombre, apellido y DNI.
- 🏢 `ClienteEmpresa`: Persona jurídica con nombre de fantasía y CUIT.

### 🏦 Tipos de cuentas:
- 💰 `CajaDeAhorro`: Cuenta con saldo y tasa de interés. Permite el cobro de intereses.
  
- 🧾 `CuentaCorriente`: Soporta giro en descubierto y depósito de cheques.
  
- 💵 `CuentaConvertibilidad`: Hereda de `CuentaCorriente`. Permite saldo en dólares y conversiones. *Solo para empresas.*

### ⚙️ Operaciones disponibles:
- ✅ Alta de clientes (individual o empresa)
- ✅ Alta de cuentas (con o sin saldo inicial)
- ✅ Depósitos y extracciones de efectivo
- 🧾 Depósito de cheques (solo cuenta corriente)
- 🔁 Conversión entre dólares y pesos (solo cuenta convertibilidad)
- 📈 Cálculo y cobro de intereses (solo caja de ahorro)
- 🧪 Validaciones estrictas (nombres, DNI, CUIT, saldos, tasas, etc.)
- 📋 Listado y selección de clientes filtrados por tipo (`instanceof`)
- 🔄 Menús interactivos para selección de operaciones
- 📊 Listado dinámico de clientes con numeración para selección

---

## 🧠 Ejemplos incluidos en pruebas

- 4 clientes predefinidos (2 individuales, 2 empresas)
- 4 cuentas predefinidas (combinadas entre tipos y clientes)
- Separación de clientes en listas filtradas por tipo (`ClienteEmpresa`, `ClienteIndividual`)
- Uso de `instanceof` con pattern matching (Java 16+) para acceder a métodos específicos

---

## 🛠️ Tecnologías utilizadas

- ☕ **Java**
- 🧩 **Lombok** (para eliminar código repetitivo como getters, setters, etc.)
- 💻 **Consola / Terminal** (interfaz por texto)
- 📝 **Programación orientada a objetos** (POO)

---

📂 Estructura del proyecto
<pre> 
  src/ 
  └── ar.org.centro8.java.curso.entidades/ 
      ├── cliente/ 
      │   ├── Cliente.java 
      │   ├── ClienteIndividual.java 
      │   └── ClienteEmpresa.java 
      └── cuenta/ 
          ├── Cuenta.java 
          ├── CajaDeAhorro.java 
          ├── CuentaCorriente.java 
          ├── CuentaConvertibilidad.java 
          └── Cheque.java 
  tests/ 
    └── TestSistemaBancario.java 
    └── TestSistemaBancarioConMenu.java
</pre>

---
## 📌 Buenas prácticas aplicadas

✅ Uso de herencia y polimorfismo para organizar jerarquía de clases

✅ Separación entre modelo de negocio y lógica de prueba / presentación

✅ Uso de Lombok para simplificar clases (menos código repetido)

✅ Código modular, mantenible y fácilmente extensible

✅ Uso de `instanceof` moderno (pattern matching) para evitar casteos innecesarios

✅ Validaciones de entrada sólidas para evitar datos inválidos

✅ Código modular, mantenible y fácilmente extensible

✅ Enumeración dinámica de clientes empresa para selección por menú
 
✅ Uso de listas genéricas (`List<Cliente>`) y separación por subtipos

---

## 🚀 Posibles mejoras futuras

- 🖥️ Interfaz gráfica (JavaFX / Swing) o web (Spring Boot)
- 💾 Persistencia de datos con base de datos (MySQL, PostgreSQL, etc.)
- 🔐 Autenticación de usuarios y roles
- 🔄 Transferencias entre cuentas
- 📊 Generación de resúmenes y estados de cuenta
- 📥 Importación / exportación de datos (CSV, JSON, XML)

---

## 📌 Requisitos recomendados

- Java 17+ (para usar `instanceof` con pattern matching)
- Lombok configurado en el IDE (IntelliJ, Eclipse, VS Code)

  ## 👨‍💻 Autor

Este proyecto fue desarrollado como ejercicio de aprendizaje de Java orientado a objetos, enfocado en diseño limpio, validaciones y estructuras de datos.

---
