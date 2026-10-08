# 🚦 Sistema de Semáforo con Raspberry Pi y Python
> *Proyecto desarrollado para la materia de Sistemas Embebidos*

---

## 📌 Descripción del Proyecto

Este repositorio contiene scripts orientados a la práctica de sistemas embebidos, destacando el control secuencial de un semáforo (LEDs rojo, amarillo y verde) mediante los pines **GPIO** de una **Raspberry Pi**, utilizando **Python** y la librería `gpiozero`. 

Incluye retardos de tiempo, gestión segura de interrupciones y prácticas complementarias de parpadeo y recorridos de luces.

---

## 🧰 Componentes Utilizados

| Componente | Cantidad | Detalle |
| :--- | :---: | :--- |
| **Raspberry Pi** | 1 | Cualquier modelo con GPIO de 40 pines |
| **LED Rojo** | 1 | Indicador de alto |
| **LED Amarillo** | 1 | Indicador de precaución |
| **LED Verde** | 1 | Indicador de avance |
| **Resistencias** | 3 | $220\Omega$ o $330\Omega$ |
| **Accesorios** | - | Protoboard y cables de conexión (Jumpers) |

---

## ⚡ Esquema de Conexiones (Pines BCM)

| Componente | Pin GPIO (Raspberry Pi) | Conexión Física |
| :--- | :---: | :--- |
| **LED Rojo** | `GPIO 17` | Ánodo $\rightarrow$ Resistencia $\rightarrow$ GPIO 17 |
| **LED Amarillo** | `GPIO 27` | Ánodo $\rightarrow$ Resistencia $\rightarrow$ GPIO 27 |
| **LED Verde** | `GPIO 22` | Ánodo $\rightarrow$ Resistencia $\rightarrow$ GPIO 22 |
| **Cátodos (GND)** | `GND` | Común a todos los LEDs |

---

## 🚀 Instalación y Ejecución

1. **Actualizar el sistema e instalar la librería GPIO:**
   ```bash
   sudo apt update
   sudo apt install python3-gpiozero
