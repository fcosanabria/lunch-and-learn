---
title: Living in the Terminal @ Datasite Lunch and Learn
sub_title: Dotfiles | Tools | Productivity
author: Francisco Sanabria
date: 2025, Julio

theme:
  override:
    footer:
      style: template
      center: "Living in the Terminal"
      left: "Francisco Sanabria, 2025. CC0"
---

### Contact

- linkedin.com/in/fcosanabria
- github.com/fcosanabria
- instagram.com/digital.death.disrupt

![spinning-rat](img/spinning-rat.gif)

<!-- end_slide -->

## CC0

![image:width:50%](img/cc-zero-2k.png)

`github.com/fcosanabria`

<!-- speaker_note: |
Copy, right? Esta presentación se encuentra publicada complememente al dominio publico. Todo lo que veran aqui como links,
imagenes y script se encuentra en mi repositorio de GitHub

Esta presentación se encuentra inspirada por NoBoilerplate.
-->
<!-- end_slide -->

# Disclaimers

- Spanglish
- Tyop
- Gazapos gramaticales
- macos = darwin = bsd = unix = posix compatible
- opt = alt
- Strong Opinions + jokes
- Tool installation ✅

<!-- speaker_note: |

- la tecla Altgr+compose key en linux es un poco complicada de usar.

- Ademas tambien se perfectamente que todo esto que van a ver aqui les va a parecer complememente inutil. Y cada que les
ensene una nueva herramienta o workflow van a pensar, y para que esto? De que me sirve?
- por que pueden serguir usando sus herramientas del dia a dia, sin ningun problema, por que son unas 10x developers.

- Y probablemente me llamen la atencion despues de esta presentacion, por dirigirme a Ustedes de manera tan despiadada y mezquina.
- Pero bueno, dejando las bromas, (no tan bromas y verdades) de lado. Espero que no se tomen las tomen a pecho. Genuinamente los quiero
un monton.

- Y si, todo lo que veran aqui, lo uso todos los dias de mi vida, en todas mis computadoras. Esto no me hace ser mejor ingeniero,
pero si me permite tener mas tiempo ~ para procrastinar aun mas.

-->

## Slides

- font: berkeley mono: https://usgraphics.com/products/berkeley-mono
  - not free
- presenterm

<!-- end_slide -->

# Keyboard Navigation

<!-- incremental_lists: true-->

<!-- speaker_note: |
- Antes de comenzar con la terminal, primero me gustaria hablar de lo mas importante: el uso del teclado para maxima efectividad
- Ustedes no saben la congoja que me da ver a la gente usan el mouse, las fechas y todo eso para navegar por el sistema operativo.
  - Claro yo entiendo el hecho de que es complememente. Ustedes se me volveran super enojados diciendo, diay? Como hago las varas,
entonces?
- Bueno, les comento las posibilidades:
-->

- CAPS LOCK 🤮
- Arrows
- Enter
- Press and Hold PopUp

<!-- end_slide -->

### Karabiner Elements

<!-- incremental_lists: true-->

- Keyboard Remapping Software

#### Examples

  <!-- speaker_note: |
    pregunta, levante la mano el que usa alt en macOS mas de 2 veces al dia que no sea para shortcups o keybindings
    -->

- Caps Lock -> Esc + Ctrl/Cmd
  - Esc + Hyper/Meh
- Remap Alt as Layer
  - I J K L (wasd motions)
  - H J K L (vim motions)
  - alt + m -> Enter (ctrl + m = ^M in Unix = "Enter" (in terminal emulations))
    - Return en Unix
  - Move around Workspaces

![keyboard](img/qwerty-example.png)

<!-- speaker_note: scan code generation y el virtual key code translation son los mismos que el de enter -->

<!-- end_slide -->

### Press and Hold

- Acentos -> hold 300ms = The worst PopUp menu ever created in human history
<!-- incremental_lists: true-->
- Alt permite realizar acentos de manera mas sencilla. (Si saben usar touchtyping lol)

#### Disable press and hold

```
defaults write -g ApplePressAndHoldEnabled -bool false

# logout or restart
```

#### Usage

```
opt + e + a
opt + e + e
opt + n + n
```

<!-- end_slide -->

# Window Manager

- Avoid using the mouse to switch windows and resizing you apps
<!-- incremental_lists: true-->
- cmd + tab = ✅ 50/50
- macos window snapping = ❌
  - stage manager

## Solution

- Tiling window manager
  - Aerospace
  - Yabai + skhd
  - Amethyst
- Snapping window manager
  - Magnet
  - Rectangle
  - Rectangle Pro

<!-- incremental_lists: false-->

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

> Combinarlas con Hyper/Meh

```
hyper + y u i o
hyper + c
hyper + m
```

<!-- column: 1 -->

![source-tiles](img/tiles.png)

<!-- end_slide -->

# Tools

## Managing Containers

# Oxker

Manage your Containers without using Docker Desktop
![oxker](img/oxker.png)

<!-- end_slide -->

## Lazydocker

![lazydocker](img/lazydocker.jpg)

<!-- end_slide -->

# DevContainers Standard

Originalmente from MS

> Rationale detrás de los devpods

- Chezmoi
- Mise
- DevContainers
  - Devpods

<!-- end_slide -->

## Text Editors

- Helix
- nvim

```zsh +exec
presemterm
```
