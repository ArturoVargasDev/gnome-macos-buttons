
# 🍎 GNOME macOS Buttons

<img src="preview.png" alt="Vista previa de los botones" width="300" align="right">

---

<a id="english"></a>
## English

### What is this?

A lightweight mod for **GNOME 45+** that replaces the standard window titlebar buttons (close, maximize, minimize) with the iconic **colored circles from macOS**.  
The symbols (✕, –, □) appear only when you hover or press the button, just like in macOS. Inactive windows show a subtle gray circle.

It works by adding a small CSS override to your GTK configuration — **your current theme (Adwaita, Yaru, adw-gtk3, etc.) stays untouched**. Only the buttons change.

### Features

- Red, yellow and green circles (close, minimize, maximize)
- Interactive states: normal, hover, active (press), backdrop (inactive window)
- Works with **GTK3** and **GTK4** applications
- No external files needed — SVGs are embedded as data URIs
- Compatible with any GTK theme
- Simple install script with automatic backup

### How it works

The mod copies two CSS files (`gtk3.css` and `gtk4.css`) into your local GTK configuration directory (`~/.config/gtk-3.0/` and `~/.config/gtk-4.0/`).  
These files override only the `headerbar` button styles, leaving the rest of your theme intact.

### Installation

1. **Download or clone the repository**  
   ```bash
   git clone https://github.com/ArturoVargasDev/gnome-macos-buttons.git
   cd gnome-macos-buttons
   ```

2. **Run the installer**  
   ```bash
   chmod +x install.sh
   ./install.sh
   ```
   The script will copy the CSS files to your `~/.config` directory.  
   If you already have custom GTK styles, a backup will be created (`.bak`).

3. **Restart your applications** or **log out and back in** to see the changes.

> 💡 No need to change your theme in GNOME Tweaks. Just run the script and you’re done.

### Uninstallation

To restore the original buttons, delete the override files:
```bash
rm ~/.config/gtk-3.0/gtk.css
rm ~/.config/gtk-4.0/gtk.css
```
If a backup was created, you can rename it back:
```bash
mv ~/.config/gtk-3.0/gtk.css.bak ~/.config/gtk-3.0/gtk.css
mv ~/.config/gtk-4.0/gtk.css.bak ~/.config/gtk-4.0/gtk.css
```

### Customization

You can edit the CSS files directly to change sizes, margins or colors. All the SVG images are embedded as **data URIs** inside the CSS, so you can replace them with your own designs.

---

<a id="español"></a>
## Español

### ¿Qué es esto?

Un mod ligero para **GNOME 45+** que reemplaza los botones estándar de la barra de título (cerrar, maximizar, minimizar) por los icónicos **círculos coloreados de macOS**.  
Los símbolos (✕, –, □) solo aparecen al pasar el ratón o al hacer clic, igual que en macOS. Las ventanas inactivas muestran un discreto círculo gris.

Funciona añadiendo un pequeño override CSS a tu configuración GTK — **tu tema actual (Adwaita, Yaru, adw-gtk3, etc.) no se modifica**. Solo cambian los botones.

### Características

- Círculos rojo, amarillo y verde (cerrar, minimizar, maximizar)
- Estados interactivos: normal, hover, activo (presionado), backdrop (ventana inactiva)
- Compatible con aplicaciones **GTK3** y **GTK4**
- No necesita archivos externos — los SVGs están incrustados como data URIs
- Funciona con cualquier tema GTK
- Instalación sencilla mediante script con backup automático

### Cómo funciona

El mod copia dos archivos CSS (`gtk3.css` y `gtk4.css`) dentro de tu directorio de configuración GTK (`~/.config/gtk-3.0/` y `~/.config/gtk-4.0/`).  
Estos archivos sobrescriben únicamente los estilos de los botones de la `headerbar`, dejando intacto el resto de tu tema.

### Instalación

1. **Descarga o clona el repositorio**  
   ```bash
   git clone https://github.com/ArturoVargasDev/gnome-macos-buttons.git
   cd gnome-macos-buttons
   ```

2. **Ejecuta el instalador**  
   ```bash
   chmod +x install.sh
   ./install.sh
   ```
   El script copiará los archivos CSS a tu directorio `~/.config`.  
   Si ya tenías estilos GTK personalizados, se creará una copia de seguridad (`.bak`).

3. **Reinicia las aplicaciones** o **cierra sesión y vuelve a entrar** para ver los cambios.

> 💡 No es necesario cambiar el tema en GNOME Tweaks. Solo ejecuta el script y listo.

### Desinstalación

Para restaurar los botones originales, elimina los archivos:
```bash
rm ~/.config/gtk-3.0/gtk.css
rm ~/.config/gtk-4.0/gtk.css
```
Si habías hecho un backup, renómbralo:
```bash
mv ~/.config/gtk-3.0/gtk.css.bak ~/.config/gtk-3.0/gtk.css
mv ~/.config/gtk-4.0/gtk.css.bak ~/.config/gtk-4.0/gtk.css
```

### Personalización

Puedes editar los archivos CSS directamente para cambiar tamaños, márgenes o colores. Todas las imágenes SVG están incrustadas como **data URIs** dentro del CSS, así que puedes reemplazarlas con tus propios diseños.

---

## 📝 License

This project is licensed under the **GNU General Public License v3.0**. See the [LICENSE](LICENSE) file for details.
```

Asegúrate de reemplazar `tuusuario` por tu nombre de usuario de GitHub y de añadir una imagen `preview.png` (o como quieras llamarla) que muestre los botones en acción.
