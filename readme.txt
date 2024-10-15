### Befehle zur Installation aller Pakete:

```bash
npm i gulp gulp-sass sass gulp-file-include gulp-clean gulp-server-livereload gulp-sourcemaps gulp-plumber gulp-notify gulp-group-css-media-queries --save-dev
```

### Beschreibung der Pakete:

- **gulp**: Das eigentliche Gulp
- **gulp-sass**: SASS/SCSS-Kompilierung
- **sass**: Erforderlich für die SASS/SCSS-Kompilierung
- **gulp-file-include**: Einbindung von Dateien ineinander. HTML include
- **gulp-clean**: Dateien löschen
- **gulp-server-livereload**: Server mit automatischer Seitenaktualisierung
- **gulp-sourcemaps**: Quellmaps für CSS
- **gulp-plumber**: Fehlerbehebung bei der Erstellung
- **gulp-notify**: Benachrichtigungen
- **gulp-group-css-media-queries**: Gruppierung von CSS-Media-Queries

---

### Skript-Erstellung. webpack, babel

#### Installation von babel:

```bash
npm i gulp-babel @babel/core @babel/preset-env
```

- **JS-Task**
- **Einstellungen in package-json**

---

### Installation von webpack:

```bash
npm i webpack-stream style-loader css-loader --save-dev
```

- **JS-Task**
- **webpack-Konfiguration**
- **Beispiel für Dateien mit Modulen**

#### Beispiel mit datepicker:

```bash
npm i air-datepicker -S
```

**JS:**

```javascript
import AirDatepicker from 'air-datepicker';
import 'air-datepicker/air-datepicker.css';

document.addEventListener('DOMContentLoaded', () => {
	new AirDatepicker('#my-element');
});
```

**HTML:**

```html
<input type="text" id="my-element">
```

---

### Bilder:

```bash
npm i gulp-imagemin@7 --save-dev
```

```javascript
.pipe(imagemin({ verbose: true }))
```

---

### Beschleunigung der Erstellung

```bash
npm install --save-dev gulp-changed
```

- **Verwendung bei Bildern, HTML, JS, CSS**

---

### web-p

```bash
npm i gulp-webp gulp-webp-html gulp-webp-css --save-dev
```