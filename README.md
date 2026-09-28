# Roadmap Q4 2026 con Supabase

## 1. Crear la base de datos
1. Crea un proyecto en https://supabase.com
2. Ve a **SQL Editor → New query**, pega el contenido de `supabase.sql` y dale **Run**.

## 2. Conectar la página
1. En Supabase ve a **Project Settings → API**.
2. Copia **Project URL** y la llave **anon public**.
3. Abre `index.html` y pégalas arriba, en `ROADMAP_CONFIG`:
   - `SUPABASE_URL`
   - `SUPABASE_ANON_KEY`

## 3. Publicar en GitHub Pages
1. Sube `index.html` a la raíz de tu repositorio.
2. **Settings → Pages →** Deploy from a branch → `main` / `(root)`.

## Cómo funciona
- La primera vez que abres la página, crea la fila del roadmap con los datos iniciales.
- Cada cambio se guarda en Supabase (y en el navegador como respaldo).
- Si otra persona tiene la página abierta, ve los cambios en vivo.
- Si no hay conexión, sigue funcionando y guarda en el navegador.

## Importante
Sin login, cualquiera que tenga el link puede editar el roadmap. Comparte el link solo con quien corresponda.
Para respaldos: **Table Editor → roadmaps →** exporta la fila como CSV/JSON.
