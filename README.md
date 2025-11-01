# 🧩 Automatic Issue Creator (GitHub Projects v2)

Aplicación web ligera en **HTML + JavaScript** que permite crear **draft issues** o **issues normales** en tus repositorios y añadirlos automáticamente a un **Project v2 de GitHub** mediante la **API GraphQL** y **REST**.

![preview](https://github.githubassets.com/images/modules/projects/project-cards.webp)

---

## 🚀 Características principales

- ✅ Crear **Draft Issues** directamente en el backlog de un **Project v2**  
- ✅ Crear **Issues normales en repositorios** y añadirlos automáticamente al Project  
- ✅ Listar tus **Projects v2** (con sus IDs `PVT_...`) visualmente  
- ✅ Soporta entrada **en texto plano o JSON**  
- ✅ Interfaz moderna, oscura y totalmente local (no envía tus datos a ningún servidor)  
- ✅ Modo interactivo: copia el `PVT_...` al campo del Project con un clic  
- ✅ No requiere instalación — basta con abrir el archivo HTML en el navegador

---

## 🧠 Cómo funciona

Esta herramienta utiliza:
- La **API GraphQL v4** de GitHub para crear `draft issues` (`addProjectV2DraftIssue`)  
- La **API REST** de GitHub para crear issues en repositorios  
- Un **token personal (PAT)** del usuario para autenticarse localmente

---

## ⚙️ Requisitos

1. Tener una cuenta en [GitHub](https://github.com)  
2. Crear un **Personal Access Token (PAT)** con permisos:
   - Para tokens *classic*:  
     - `repo`  
     - `read:org`  
     - `project`  
   - Para tokens *fine-grained*:  
     - Acceso al repositorio o la organización que contiene el Project  
     - Permisos **Read & Write en Projects**

👉 Genera o gestiona tus tokens aquí: [https://github.com/settings/tokens](https://github.com/settings/tokens)

> ⚠️ Si el Project pertenece a una organización, recuerda **autorizar el token (Enable SSO)** para esa org.

---

## 🧩 Instrucciones de uso

1. **Descarga o clona** el proyecto:
   ```bash
   git clone https://github.com/yancep/AutomaticIssueCreator.git
   cd AutomaticIssueCreator