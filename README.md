# 💳 Sistema Bancario - Proyecto Java

## 🧾 Descripción

Este proyecto en **Java** simula un sistema bancario orientado a objetos. Incluye diferentes tipos de **clientes** y **cuentas bancarias**, con funcionalidades básicas como:

- Gestión de saldos
- Depósitos y extracciones
- Manejo de cheques
- Conversión entre pesos y dólares

---

## 🧠 Funcionalidades principales

### 👥 Tipos de clientes:
- 🧑 `ClienteIndividual`
- 🏢 `ClienteEmpresa`

### 🏦 Tipos de cuentas:
- 💰 `CajaDeAhorro`  
  Cuenta de ahorro con tasa de interés.
  
- 🧾 `CuentaCorriente`  
  Permite giro en descubierto y depósito de cheques.
  
- 💵 `CuentaConvertibilidad`  
  Extiende cuenta corriente, permite manejar saldo en dólares y conversiones entre monedas. *(Exclusiva para empresas)*

### ⚙️ Operaciones disponibles:
- ✅ Depósitos y extracciones de efectivo
- 🧾 Depósito de cheques (solo en cuenta corriente)
- 🔁 Conversión entre dólares y pesos (solo en cuenta convertibilidad)
- 📈 Cálculo y cobro de intereses (solo en caja de ahorro)

---

## 🛠️ Tecnologías utilizadas

- ☕ **Java**
- 🧩 **Lombok** (para eliminar código repetitivo: getters, setters, etc.)
- 💻 **Consola / Terminal** (para pruebas y ejecución)

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
</pre>

---
## 📌 Buenas prácticas aplicadas

✅ Uso de herencia y polimorfismo para organizar jerarquía de clases

✅ Separación entre modelo de negocio y lógica de prueba / presentación

✅ Uso de Lombok para simplificar clases (menos código repetido)

✅ Código modular, mantenible y fácilmente extensible

---

## 🚀 Posibles mejoras futuras

🖥️ Interfaz gráfica (Swing, JavaFX) o web (Spring Boot)

💾 Persistencia de datos con base de datos (MySQL, PostgreSQL, etc.)

🔄 Transferencias entre cuentas

📊 Generación de resúmenes y estados de cuenta

🔐 Autenticación de usuarios

---
