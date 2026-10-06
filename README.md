# Relevamiento Comercial SCN

Versión minimalista con app móvil y panel de supervisor en tiempo real.

## Fuente vigente
- `LISTA_DE_CLIENTES_ACTIVOS.xlsx`
- Registros preparados: 2040
- No se utiliza "Aplicación SCN.xlsx".

## Instalación
1. Crear el proyecto en Supabase.
2. Ejecutar `supabase/01_schema.sql`.
3. Importar `data/clientes_supabase.csv` en la tabla `clientes`.
4. Publicar todo el contenido en GitHub Pages.
5. Configurar Project URL y clave pública desde la aplicación.
6. Panel supervisor: `/supervisor/`.

## Seguridad
Las políticas anónimas incluidas permiten una prueba rápida. Para producción, activar Supabase Auth y limitar las políticas a usuarios autenticados. Nunca usar la clave service_role en GitHub Pages.

## V2 estable
Incluye modo demo local, navegación corregida, validaciones visibles, botones con tipo explícito, configuración persistente, panel supervisor y reporte de pruebas.

## Opción OTROS
La pregunta 1 incluye OTROS. Al seleccionarla, se habilita un campo obligatorio para especificar el rubro. Si la tabla visitas ya existe, ejecutar `supabase/02_agregar_tipo_negocio_otro.sql`.
