# 🚀 Guía de Integración CRM FERROTODO con Google Sheets & Semilla Automática

Esta solución permite que tus ejecutivos administren prospectos en tiempo real desde [`index.html`](file:///c:/xampp/htdocs/VISITAS/index.html) durante la Expocruz, realizando operaciones **CRUD completas** (Crear, Leer, Editar, Eliminar y Sembrar datos) en tu propia hoja de cálculo de Google Sheets.

---

## 📌 Paso 1: Crear tu Google Sheet
1. Abre [Google Sheets](https://sheets.google.com) y crea una nueva Hoja de Cálculo.
2. Nómbrala: **"FERROTODO - CRM Comercial Expocruz 2026"**.

---

## 📌 Paso 2: Pegar el Código en Apps Script
1. En el menú superior de tu Google Sheet, ve a: **Extensiones > Apps Script**.
2. Borra todo el código por defecto en `Código.gs`.
3. Abre el archivo local [`google_sheets_script.js`](file:///c:/xampp/htdocs/VISITAS/google_sheets_script.js), copia todo su contenido y pégalo en Apps Script.
4. Haz clic en el **Disco (Guardar)** o presiona `Ctrl + S`.

---

## 📌 Paso 3: Sembrar / Poblar la Data Inicial (1 Clic)
1. En la barra superior del editor de Apps Script, selecciona la función **`seedInitialData`** en la lista desplegable.
2. Haz clic en **Ejecutar**.
3. ¡Listo! Apps Script creará automáticamente 4 pestañas profesionalmente diseñadas con los colores de FERROTODO:
   - 📊 **`Dashboard CRM`**: Tarjetas de KPIs, fórmulas de avance y cobertura comercial.
   - 🏢 **`Catálogo Empresas`**: Precargado con las **308 empresas verificadas** distribuidas por vendedor y fecha.
   - 🔥 **`Prospectos Capturados`**: Hoja activa de recepción de datos del CRM.
   - 👤 **`Vendedores & Sectores`**: Cartera por ejecutivo comercial y dupla de campo.

---

## 📌 Paso 4: Publicar como Aplicación Web (API Webhook CRUD)
1. En Apps Script, haz clic en **Implementar > Nueva implementación**.
2. Tipo: **Aplicación web**.
3. Parámetros:
   - **Descripción**: `FERROTODO CRM Webhook CRUD`
   - **Ejecutar como**: `Yo` (tu correo de Google)
   - **Quién tiene acceso**: **`Cualquier persona`** *(OBLIGATORIO para permitir recibir los prospectos del HTML)*
4. Haz clic en **Implementar**, concede los permisos requeridos y copia la **URL de la aplicación web** (empieza con `https://script.google.com/macros/s/.../exec`).

---

## 📌 Paso 5: Conectar en la App HTML FERROTODO
1. Abre [`index.html`](file:///c:/xampp/htdocs/VISITAS/index.html) en tu navegador.
2. Haz clic en el botón **`⚙️ Conectar Google Sheets`** en la barra superior.
3. Pega la URL de tu aplicación web y haz clic en **Guardar Configuración**.
4. *(Opcional)* También puedes hacer clic en **`🌱 Poblar / Sembrar Google Sheets`** directamente desde el modal para inicializar tu hoja a distancia.

---

## 🛠️ Operaciones CRUD Habilitadas:
- ➕ **CREAR**: Al hacer clic en `+ Ficha CRM` o `+ Prospecto Fuera de Lista`.
- ✏️ **EDITAR**: Editar cualquier ficha comercial o cambiar de vendedor/día.
- 🗑️ **ELIMINAR**: Eliminar prospectos descartados directamente desde la vista CRM.
- 🌱 **SEMBRAR / SEED**: Sembrado de 308 empresas iniciales + 6 ejecutivos comerciales.
