# Control Móvil

App Android para controlar el uso del móvil y bloquear apps y webs.

## Qué hace

- **Tiempo de pantalla** de hoy y de los últimos 7 días (con gráfico).
- **Desbloqueos** al día y media de tiempo por desbloqueo.
- **Apps más usadas** (top 10 del día).
- **Bloquear apps**: siempre, o con límite diario (15 min, 30 min, 1 h, 2 h).
- **Bloquear webs** (instagram.com, youtube.com…) en Chrome, Samsung Internet,
  Firefox, Edge, Brave, Opera, Vivaldi y DuckDuckGo.
- Interruptor general para pausar todos los bloqueos.

Todo se queda en el móvil: no hay internet, cuentas ni anuncios.

## Cómo conseguir el APK

### Opción A — GitHub (sin instalar nada en el ordenador)
1. Crea una cuenta en github.com y un repositorio nuevo (puede ser privado).
2. «Add file → Upload files» y arrastra **todo el contenido** de esta carpeta
   (incluida la carpeta `.github`).
3. Ve a la pestaña **Actions**: se compila solo en unos 5 minutos.
4. Abre la ejecución terminada → abajo, en *Artifacts*, descarga `ControlMovil-apk`.
   Es un .zip con `app-debug.apk` dentro.

### Opción B — Android Studio
1. Instala Android Studio y abre esta carpeta (File → Open).
2. Espera a que termine de sincronizar.
3. Build → Build App Bundle(s) / APK(s) → Build APK(s).
4. El APK queda en `app/build/outputs/apk/debug/app-debug.apk`.

## Instalar y activar en el móvil

1. Pasa el APK al móvil y ábrelo. Permite «instalar apps desconocidas» cuando lo pida.
2. Abre **Control Móvil** → «Dar acceso» → activa Control Móvil en *Acceso a datos de uso*.
3. Antes de activar el bloqueador (Android 13 o superior):
   Ajustes → Aplicaciones → Control Móvil → menú ⋮ → **Permitir ajustes restringidos**.
4. Vuelve a la app → «Abrir Accesibilidad» → Apps instaladas → Control Móvil → activar.
5. Samsung/Xiaomi: quita la optimización de batería de la app para que el bloqueador
   no se cierre solo (Ajustes → Batería → Control Móvil → Sin restricciones).

## Notas

- Los números pueden diferir algo de Bienestar digital: se cuenta el tiempo de cada
  app en primer plano (sin contar la pantalla de inicio).
- Los límites diarios se comprueban cada ~30 s, así que pueden pasarse unos segundos.
