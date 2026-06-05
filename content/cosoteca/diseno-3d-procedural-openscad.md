+++
title = "Diseño 3D procedural con OpenSCAD"
description = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Introducción al modelado paramétrico y generativo usando OpenSCAD para fabricación digital."
date = 2026-06-05
+++

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## ¿Qué es OpenSCAD?

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Praesent mauris.

Fusce nec tellus sed augue semper porta. Mauris massa. Vestibulum lacinia arcu eget nulla. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos hymenaeos.

## Conceptos fundamentales

Curabitur sodales ligula in libero. Sed dignissim lacinia nunc. Curabitur tortor. Pellentesque nibh. Aenean quam. In scelerisque sem at dolor. Maecenas mattis. Sed convallis tristique sem.

### Primitivas geométricas

Proin ut ligula vel nunc egestas porttitor. Morbi lectus risus, iaculis vel, suscipit quis, luctus non, massa. Fusce ac turpis quis ligula lacinia aliquet. Mauris ipsum.

```scad
// Lorem ipsum: cubo paramétrico
module caja(ancho, alto, profundo) {
    cube([ancho, profundo, alto]);
}

caja(ancho=30, alto=20, profundo=15);
```

### Operaciones booleanas

Nulla metus metus, ullamcorper vel, tincidunt sed, euismod in, nibh. Quisque volutpat condimentum velit. Class aptent taciti sociosqu ad litora torquent per conubia nostra.

```scad
// Lorem ipsum: diferencia booleana
difference() {
    cube([40, 40, 40]);
    translate([5, 5, 5])
        cube([30, 30, 30]);
}
```

### Módulos y parámetros

Nam nec ante. Sed lacinia, urna non tincidunt mattis, tortor neque adipiscing diam, a cursus ipsum ante quis turpis. Nunc massa justo, ultrices id velit sit amet, condimentum congue felis.

```scad
// Lorem ipsum: módulo reutilizable
module perforacion(radio=5, profundo=10) {
    cylinder(h=profundo, r=radio, center=true);
}
```

## Diseño procedural

Donec vestibulum lorem quis erat elementum, et tincidunt dui tincidunt. Nullam maximus orci eu dui tristique, at efficitur arcu commodo. Phasellus feugiat arcu a felis dignissim, vel bibendum nisi accumsan.

Aliquam erat volutpat. Vivamus efficitur nunc in libero convallis, at ullamcorper felis ultrices. Sed malesuada risus at orci bibendum, id varius enim laoreet.

### Iteración con bucles

```scad
// Lorem ipsum: grilla de cilindros
for (x = [0:10:50]) {
    for (y = [0:10:50]) {
        translate([x, y, 0])
            cylinder(h=8, r=3);
    }
}
```

### Funciones matemáticas

Curabitur sodales ligula in libero. Sed dignissim lacinia nunc. Curabitur tortor. Pellentesque nibh. Aenean quam. In scelerisque sem at dolor. Maecenas mattis.

## Exportación para fabricación

Sed convallis tristique sem. Proin ut ligula vel nunc egestas porttitor. Morbi lectus risus, iaculis vel, suscipit quis, luctus non, massa. Fusce ac turpis quis ligula lacinia aliquet.

- **STL** — Lorem ipsum dolor sit amet para impresión 3D FDM y SLA
- **DXF** — Consectetur adipiscing elit para corte láser y CNC
- **SVG** — Sed do eiusmod tempor para rutas vectoriales

## Recursos adicionales

Mauris ipsum. Nulla metus metus, ullamcorper vel, tincidunt sed, euismod in, nibh. Quisque volutpat condimentum velit. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos hymenaeos.
