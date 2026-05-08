# 🤝 Guia de Contribucion

Gracias por querer contribuir al Banco de Examenes de la AECCI. Este archivo explica como hacerlo paso a paso.

No es necesario ser experto en Git, si es preferible se pueden enviar los archivos por correo y se suben manualmente.

---

## ¿Que se puede contribuir?

| Permitido | No permitido |
|---|---|
| Examenes de ciclos anteriores | Material con derechos de autor (libros, articulos pagos) |
| Apuntes y resumenes propios | Soluciones de tareas o proyectos en curso |
| Diapositivas de cursos | Informacion personal de estudiantes o profesores |
| Proyectos y enunciados de ciclos pasados | Material de ciclos que aun no han finalizado |
| Quices y evaluaciones anteriores | Archivos ejecutables o con contenido malicioso |

---

## Estructura del repositorio

Los cursos estan organizados de la siguiente manera:

```
Año_<X>
  └── Ciclo_<X>
     └── <Nombre_curso>_<Código_curso>
```

**Ejemplo:**
```
Año_1
 └── Ciclo_1
    ├── Introduccion_a_la_computacion_CI0110
    └── Introduccion_a_la_matematica_para_computacion_MA0291
```

Los **archivos** están organizados de la siguiente manera:


Ruta ejemplo: `Año_1/Ciclo_2/Programacion_I_CI0112/2025_Semestre_I/`
```
2025_Semestre_I/
├── Carta_al_Estudiante_CI0112_I_2025.pdf
├── 01_Material/
│   ├── Tema_01_Punteros.pdf
│   ├── Tema_02_Memoria_Dinamica.pdf
│   └── Tema_03_Estructuras.pdf
├── 02_Quices/
│   ├── Quiz_1_Enunciado.pdf
│   ├── Quiz_2_Enunciado.pdf
│   └── Quiz_3_Enunciado.pdf
└── 03_Examenes_Enunciados/
    ├── Parcial_1_Enunciado.pdf
    ├── Parcial_2_Enunciado.pdf
    └── Final_Enunciado.pdf
```

**Tipos de archivo sugeridos para el nombre:**
- `examen_` -- examenes y quices
- `apuntes_` -- apuntes y resumenes
- `slides_` -- diapositivas
- `proyecto_` -- enunciados de proyectos
- `practica_` -- ejercicios de practica

---

## 🚀 Como contribuir

### Opcion A -- Por correo electronico (más facil)

Si no usas Git o preferis una forma mas directa, envia tus archivos a:

**esteban.baires@ucr.ac.cr**

Incluye en el correo:
- El nombre del curso y su codigo (ej: CI-1310 Bases de Datos)
- El año y ciclo al que pertenece el material (ej: 2024 I Ciclo)
- Una breve descripcion de lo que estas enviando
- Los archivos adjuntos en **formato PDF** de preferencia

---

### Opcion B -- Via GitHub Issue (sin Git)

Si no sabes usar Git todavia, abri un [Issue](../../issues) con:
- El curso al que pertenece el material
- El anio y ciclo
- Una descripcion de lo que queres subir

---

### Opcion C -- Pull Request (recomendado para usuarios de Git)

1. **Hacer un fork** de este repositorio usando el boton "Fork" en GitHub

2. **Clonar tu fork** en tu computadora:
   ```bash
   git clone https://github.com/<tu-usuario>/banco_examenes.git
   ```

3. **Crea una rama** con un nombre descriptivo:
   ```bash
   git checkout -b agregar/CI-1310-examen-2024-I
   ```

4. **Agrega tus archivos** en la carpeta correspondiente segun la estructura del repositorio

5. **Hace commit** de tus cambios:
   ```bash
   git add .
   git commit -m "Agrega examen parcial 1 de CI-1310 - 2024 I ciclo"
   ```

6. **Subi tu rama** a tu fork:
   ```bash
   git push origin agregar/CI-1310-examen-2024-I
   ```

7. **Abri un Pull Request** desde tu fork hacia la rama `main` de este repositorio

---

## ¿Que pasa despues?

1. Un mantenedor del repositorio revisara la contribucion
2. Si todo esta en orden, se aprobará y se unirá a `main`
3. Una vez mergeado, **el CI/CD lo despliega automáticamente** en un par de minutos -- no hace falta hacer nada más

El proceso puede de revisión puede tardar algunos dias dependiendo de la disponibilidad.

---

## Buenas practicas

- Usar nombres de archivo descriptivos y sin espacios (usar guiones bajos `_`)
- Preferibles archivos en formato **PDF** para mayor compatibilidad
- Si el archivo tiene soluciones, indicarlo en el nombre: `examen_parcial1_con_soluciones.pdf`
- Un Pull Request por curso o tema es mas facil de revisar que uno con muchos archivos mezclados

---

## ❓ Preguntas frecuentes

**¿Puedo subir material de un profesor sin su permiso?**
Si el material fue distribuido publicamente durante el curso (por ejemplo, en un aula virtual), generalmente esta bien. Si tenes dudas, pregunta antes de subir.

**¿Puedo subir materiales de cursos fuera de la ECCI?**
Por ahora el archivo esta enfocado en la ECCI-UCR. Abri un Issue si queres discutirlo.

**¿Que hago si subi algo por error?**
Abri un Issue indicando que archivo queres remover y lo atenderemos a la brevedad. O envia un correo a esteban.baires@ucr.ac.cr.

---

*¿Tenes preguntas que no estan aqui? Abri un [Issue](../../issues) o escribe a esteban.baires@ucr.ac.cr*
