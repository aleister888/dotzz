<img src="https://wiki.installgentoo.com/images/f/f9/Arch-linux-logo.png" align="left" height="90px" hspace="10px" vspace="0px">

### Arch Linux - dotfiles

---

Auto-instalador de Arch Linux con dwm, dmenu y mi configuración personal.

<p float="center">
<img src="https://raw.githubusercontent.com/aleister888/arch-installer/refs/heads/main/assets/screenshots/screenshot1.jpg" width="49%" />
<img src="https://raw.githubusercontent.com/aleister888/arch-installer/refs/heads/main/assets/screenshots/screenshot2.jpg" width="49%" />
</p>

---

#### Instalación

- Ejecuta como root:

```bash
bash <(curl https://raw.githubusercontent.com/aleister888/arch-installer/main/install.sh)
```

> [!NOTE]
> La instalación toma unos `30-45 minutos` aproximadamente.

---

#### Características

- **LUKS y LVM**: `swap` y `/` encriptados (`/boot` sin encriptar)
- Compatible solo con **UEFI**.
- Configuración automática de `Xorg` y `eww` basada en el DPI y la resolución.
- Entorno limpio y organizado según el estándar [XDG Base Directory](https://wiki.archlinux.org/title/XDG_Base_Directory).

---

#### Importante: Preparación del disco para encriptación

> [!CAUTION]
> Si activas la encriptación, **limpia el disco antes de usar el instalador** para proteger los datos residuales:
>
> ```bash
> dd if=/dev/urandom of=/dev/sdX
> ```
>
> Este proceso puede tardar horas según el tamaño del disco.

##### Alternativa

Tras la instalación, llena el espacio con un archivo temporal:

```bash
dd if=/dev/zero of=/home/usuario/archivo
```

Más detalles en: [Arch Wiki - dm-crypt](https://wiki.archlinux.org/title/Dm-crypt/Drive_preparation)

---

#### Créditos y Referencias

Agradecimientos especiales a:

- [Luke Smith](https://github.com/LukeSmithxyz) por la inspiración y sus scripts.
- [suckless.org](https://suckless.org) por las herramientas utilizadas.
