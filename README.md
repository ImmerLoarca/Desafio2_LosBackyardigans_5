# 🚀 Desafío - Optimización de la Infraestructura de Red de TechSolutions Inc.

Repositorio oficial del **Equipo 5 - LosBackyardigans** para la asignatura  
**Administración e Implementación de Servicios de Red con Sistemas Operativos Libres (ASI104)**,  
Universidad Don Bosco, Ciclo 02/2025.  

Este proyecto corresponde al **Caso de Estudio: Optimización de la Infraestructura de Red de TechSolutions Inc.**,  
donde se analizan las principales problemáticas de la red corporativa y se presentan soluciones técnicas y documentadas.  

---

## 📌 Objetivo General
Diseñar un plan de acción integral que **diagnostique y resuelva los problemas de infraestructura, seguridad y gestión de software de TechSolutions Inc.**, garantizando una red **estable, eficiente, segura y escalable**.

---

## 🎯 Objetivos Específicos
- Analizar los problemas críticos en almacenamiento, gestión de paquetes, configuración de red y seguridad.  
- Proponer soluciones técnicas que apliquen buenas prácticas en administración de sistemas Linux.  
- Documentar de forma clara y estandarizada la solución en **Markdown** dentro de un repositorio GitHub.  
- Fomentar el trabajo colaborativo simulando un equipo real de TI empresarial.  

---

## 👥 Integrantes del Equipo 5 - *LosBackyardigans*

| Integrante                          | Sección Responsable                              |
|------------------------------------|-------------------------------------------------|
| **Mauricio Manuel Alvarado Rivera** | [Gestión de Paquetes](packages.md) |
| **Bryan Josué Díaz Ascencio**       | [Almacenamiento](storage.md) |
| **Diego Alberto Fuentes Osorio**    | [Seguridad](security.md) |
| **Immer Manuel Loarca Santos**      | [Gestión de Paquetes - explicación adicional](packages.md) |
| **Javier Stanley Escobar Portillo** | [Configuración de Red](networking.md) |

---

## 🛠️ Contenido del Repositorio
Este repositorio se organiza en secciones independientes, cada una enfocada en una problemática específica:

- 📂 **[storage.md](storage.md):**  
  Explica los riesgos de fallos de disco y propone la implementación de **RAID 5** para mejorar la redundancia y disponibilidad de los datos.

- 📂 **[Packages.md](Packages.md):**  
  Detalla los problemas de instalar paquetes manualmente y presenta la solución mediante **repositorios espejo (mirrors)**, incluyendo ejemplos de comandos.

- 📂 **[networking.md](networking.md):**  
  Analiza las limitaciones del modo NAT en VirtualBox, compara con **Puente y Red Interna**, y propone el uso de **Bridge Adapter con IP estática** para entornos colaborativos.

- 📂 **[security.md](security.md):**  
  Identifica vulnerabilidades y documenta la configuración de **UFW (Uncomplicated Firewall)** para restringir accesos, con reglas específicas de SSH.

---

## 📊 Plan de Acción General
El trabajo se organizó en **4 fases principales**:

1. 🔍 **Diagnóstico** – Identificación de las deficiencias en la infraestructura actual.  
2. 💡 **Diseño de Soluciones** – Selección de herramientas y metodologías adecuadas (RAID, mirrors, UFW, bridge networking).  
3. 🛠️ **Documentación Técnica** – Redacción de procedimientos detallados en Markdown con ejemplos de comandos.  
4. ✅ **Validación y Conclusiones** – Evaluación de los beneficios y comparación con el estado actual.  

---

## 📂 Instrucciones de Uso del Repositorio
1. Clonar el repositorio con Git:  
   ```bash
   git clone https://github.com/LosBackyardigans/Desafio_Equipo5.git
