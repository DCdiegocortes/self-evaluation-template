# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 0 correctas de 20 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,7 @@
-apellido1 | apellido2 | nombre
-Domínguez | Guerrero | Antonio
-Gea | Ruiz | Sonia
-Gutiérrez | López | Juan
-Heller | Pagac | Pedro
-Herman | Pacocha | Daniel
-Hernández | Martínez | Irene
-Herzog | Tremblay | Ramón
-Koss | Bayer | José
-Lakin | Yundt | Inma
-Saez | Vega | Juan
-Sánchez | Pérez | Salvador
-Strosin | Turcotte | Ismael
+nombre
+Inma
+Irene
+Juan
+Pedro
+Salvador
+Sonia
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 2: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,2 @@
-nombre | apellido1 | apellido2
-Pedro | Heller | Pagac
-Ismael | Strosin | Turcotte
+nombre | telefono
+Pedro | NULL
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1 @@
-id | nombre | apellido1 | apellido2 | fecha_nacimiento
-7.00 | Ismael | Strosin | Turcotte | 1999-05-24
-22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
+nombre
```

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 4: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-nombre | apellido1 | apellido2 | nif
-Antonio | Fahey | Considine | 10485008K
-Guillermo | Ruecker | Upton | 85869555K
+nombre | telefono | nif
+Antonio | NULL | 10485008K
+Guillermo | NULL | 85869555K
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,52 @@
-id | nombre | cuatrimestre | curso | id_grado
-72.00 | Bases moleculares del desarrollo vegetal | 1.00 | 3.00 | 7.00
-73.00 | Fisiología animal | 1.00 | 3.00 | 7.00
-74.00 | Metabolismo y biosíntesis de biomoléculas | 1.00 | 3.00 | 7.00
-75.00 | Operaciones de separación | 1.00 | 3.00 | 7.00
-76.00 | Patología molecular de plantas | 1.00 | 3.00 | 7.00
-77.00 | Técnicas instrumentales básicas | 1.00 | 3.00 | 7.00
+nombre
+Álgegra lineal y matemática discreta
+Cálculo
+Física para informática
+Introducción a la programación
+Organización y gestión de empresas
+Estadística
+Estructura y tecnología de computadores
+Fundamentos de electrónica
+Lógica y algorítmica
+Metodología de la programación
+Arquitectura de Computadores
+Estructura de Datos y Algoritmos I
+Ingeniería del Software
+Sistemas Inteligentes
+Sistemas Operativos
+Bases de Datos
+Estructura de Datos y Algoritmos II
+Fundamentos de Redes de Computadores
+Planificación y Gestión de Proyectos Informáticos
+Programación de Servicios Software
+Desarrollo de interfaces de usuario
+Ingeniería de Requisitos
+Integración de las Tecnologías de la Información en las Organizaciones
+Modelado y Diseño del Software 1
+Multiprocesadores
+Seguridad y cumplimiento normativo
+Sistema de Información para las Organizaciones
+Tecnologías web
+Teoría de códigos y criptografía
+Administración de bases de datos
+Herramientas y Métodos de Ingeniería del Software
+Informática industrial y robótica
+Ingeniería de Sistemas de Información
+Modelado y Diseño del Software 2
+Negocio Electrónico
+Periféricos e interfaces
+Sistemas de tiempo real
+Tecnologías de acceso a red
+Tratamiento digital de imágenes
+Administración de redes y sistemas operativos
+Almacenes de Datos
+Fiabilidad y Gestión de Riesgos
+Líneas de Productos Software
+Procesos de Ingeniería del Software 1
+Tecnologías multimedia
+Análisis y planificación de las TI
+Desarrollo Rápido de Aplicaciones
+Gestión de la Calidad y de la Innovación Tecnológica
+Inteligencia del Negocio
+Procesos de Ingeniería del Software 2
+Seguridad Informática
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_grado

---

## ❌ Query 6: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
-apellido1 | apellido2 | nombre | departamento
-Fahey | Considine | Antonio | Economía y Empresa
-Hamill | Kozey | Manolo | Informática
-Kohler | Schoen | Alejandro | Matemáticas
-Lemke | Rutherford | Cristina | Economía y Empresa
-Monahan | Murray | Micaela | Agronomía
-Ramirez | Gea | Zoe | Informática
-Ruecker | Upton | Guillermo | Educación
-Schmidt | Fisher | David | Matemáticas
-Schowalter | Muller | Francesca | Química y Física
-Spencer | Lakin | Esther | Educación
-Stiedemann | Morissette | Alfredo | Química y Física
-Streich | Hirthe | Carmen | Educación
+nombre | nombre
+Zoe | Informática
+Manolo | Informática
+David | Matemáticas
+Alejandro | Matemáticas
+Cristina | Economía y Empresa
+Antonio | Economía y Empresa
+Esther | Educación
+Carmen | Educación
+Guillermo | Educación
+Micaela | Agronomía
+Alfredo | Química y Física
+Francesca | Química y Física
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | anyo_inicio | anyo_fin
-Álgegra lineal y matemática discreta | 2014.00 | 2015.00
-Cálculo | 2014.00 | 2015.00
-Física para informática | 2014.00 | 2015.00
+nombre
+Álgegra lineal y matemática discreta
+Cálculo
+Física para informática
```

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura, PRIMARY,nif

---

## ❌ Query 8: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,13 @@
-nombre
-Informática
+apellido1 | apellido2 | nombre | nombre
+Ramirez | Gea | Zoe | Informática
+Hamill | Kozey | Manolo | Informática
+Schmidt | Fisher | David | Matemáticas
+Kohler | Schoen | Alejandro | Matemáticas
+Lemke | Rutherford | Cristina | Economía y Empresa
+Fahey | Considine | Antonio | Economía y Empresa
+Spencer | Lakin | Esther | Educación
+Streich | Hirthe | Carmen | Educación
+Ruecker | Upton | Guillermo | Educación
+Monahan | Murray | Micaela | Agronomía
+Stiedemann | Morissette | Alfredo | Química y Física
+Schowalter | Muller | Francesca | Química y Física
```

⏱ Tiempo: 0.27 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 9: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1 @@
-nombre | apellido1 | apellido2
-Inma | Lakin | Yundt
-Irene | Hernández | Martínez
-Sonia | Gea | Ruiz
+apellido1 | apellido2 | nombre
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,4 @@
-departamento | apellido1 | apellido2 | nombre
-Agronomía | Monahan | Murray | Micaela
-Economía y Empresa | Fahey | Considine | Antonio
-Economía y Empresa | Lemke | Rutherford | Cristina
-Educación | Ruecker | Upton | Guillermo
-Educación | Spencer | Lakin | Esther
-Educación | Streich | Hirthe | Carmen
-Informática | Hamill | Kozey | Manolo
-Informática | Ramirez | Gea | Zoe
-Matemáticas | Kohler | Schoen | Alejandro
-Matemáticas | Schmidt | Fisher | David
-Química y Física | Schowalter | Muller | Francesca
-Química y Física | Stiedemann | Morissette | Alfredo
+nombre
+Filología
+Derecho
+Biología y Geología
```

⏱ Tiempo: 0.22 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 11: Error
- **Descripción**: 1054 (42S22): Unknown column 'P.id_profesor' in 'on clause'


## ❌ Query 12: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,63 @@
 nombre
-Filología
-Derecho
-Biología y Geología
+Ingeniería de Requisitos
+Integración de las Tecnologías de la Información en las Organizaciones
+Modelado y Diseño del Software 1
+Multiprocesadores
+Seguridad y cumplimiento normativo
+Sistema de Información para las Organizaciones
+Tecnologías web
+Teoría de códigos y criptografía
+Administración de bases de datos
+Herramientas y Métodos de Ingeniería del Software
+Informática industrial y robótica
+Ingeniería de Sistemas de Información
+Modelado y Diseño del Software 2
+Negocio Electrónico
+Periféricos e interfaces
+Sistemas de tiempo real
+Tecnologías de acceso a red
+Tratamiento digital de imágenes
+Administración de redes y sistemas operativos
+Almacenes de Datos
+Fiabilidad y Gestión de Riesgos
+Líneas de Productos Software
+Procesos de Ingeniería del Software 1
+Tecnologías multimedia
+Análisis y planificación de las TI
+Desarrollo Rápido de Aplicaciones
+Gestión de la Calidad y de la Innovación Tecnológica
+Inteligencia del Negocio
+Procesos de Ingeniería del Software 2
+Seguridad Informática
+Biologia celular
+Física
+Matemáticas I
+Química general
+Química orgánica
+Biología vegetal y animal
+Bioquímica
+Genética
+Matemáticas II
+Microbiología
+Botánica agrícola
+Fisiología vegetal
+Genética molecular
+Ingeniería bioquímica
+Termodinámica y cinética química aplicada
+Biorreactores
+Biotecnología microbiana
+Ingeniería genética
+Inmunología
+Virología
+Bases moleculares del desarrollo vegetal
+Fisiología animal
+Metabolismo y biosíntesis de biomoléculas
+Operaciones de separación
+Patología molecular de plantas
+Técnicas instrumentales básicas
+Bioinformática
+Biotecnología de los productos hortofrutículas
+Biotecnología vegetal
+Genómica y proteómica
+Procesos biotecnológicos
+Técnicas instrumentales avanzadas
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 13: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,2 @@
-apellido1 | apellido2 | nombre
-Schmidt | Fisher | David
-Kohler | Schoen | Alejandro
-Lemke | Rutherford | Cristina
-Fahey | Considine | Antonio
-Spencer | Lakin | Esther
-Streich | Hirthe | Carmen
-Ruecker | Upton | Guillermo
-Monahan | Murray | Micaela
-Stiedemann | Morissette | Alfredo
-Schowalter | Muller | Francesca
+total
+12.00
```

⏱ Tiempo: 0.22 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 14: Incorrecto
```diff
--- 
+++ 
@@ -1,63 +1,7 @@
-id | nombre
-22.00 | Ingeniería de Requisitos
-23.00 | Integración de las Tecnologías de la Información en las Organizaciones
-24.00 | Modelado y Diseño del Software 1
-25.00 | Multiprocesadores
-26.00 | Seguridad y cumplimiento normativo
-27.00 | Sistema de Información para las Organizaciones
-28.00 | Tecnologías web
-29.00 | Teoría de códigos y criptografía
-30.00 | Administración de bases de datos
-31.00 | Herramientas y Métodos de Ingeniería del Software
-32.00 | Informática industrial y robótica
-33.00 | Ingeniería de Sistemas de Información
-34.00 | Modelado y Diseño del Software 2
-35.00 | Negocio Electrónico
-36.00 | Periféricos e interfaces
-37.00 | Sistemas de tiempo real
-38.00 | Tecnologías de acceso a red
-39.00 | Tratamiento digital de imágenes
-40.00 | Administración de redes y sistemas operativos
-41.00 | Almacenes de Datos
-42.00 | Fiabilidad y Gestión de Riesgos
-43.00 | Líneas de Productos Software
-44.00 | Procesos de Ingeniería del Software 1
-45.00 | Tecnologías multimedia
-46.00 | Análisis y planificación de las TI
-47.00 | Desarrollo Rápido de Aplicaciones
-48.00 | Gestión de la Calidad y de la Innovación Tecnológica
-49.00 | Inteligencia del Negocio
-50.00 | Procesos de Ingeniería del Software 2
-51.00 | Seguridad Informática
-52.00 | Biologia celular
-53.00 | Física
-54.00 | Matemáticas I
-55.00 | Química general
-56.00 | Química orgánica
-57.00 | Biología vegetal y animal
-58.00 | Bioquímica
-59.00 | Genética
-60.00 | Matemáticas II
-61.00 | Microbiología
-62.00 | Botánica agrícola
-63.00 | Fisiología vegetal
-64.00 | Genética molecular
-65.00 | Ingeniería bioquímica
-66.00 | Termodinámica y cinética química aplicada
-67.00 | Biorreactores
-68.00 | Biotecnología microbiana
-69.00 | Ingeniería genética
-70.00 | Inmunología
-71.00 | Virología
-72.00 | Bases moleculares del desarrollo vegetal
-73.00 | Fisiología animal
-74.00 | Metabolismo y biosíntesis de biomoléculas
-75.00 | Operaciones de separación
-76.00 | Patología molecular de plantas
-77.00 | Técnicas instrumentales básicas
-78.00 | Bioinformática
-79.00 | Biotecnología de los productos hortofrutículas
-80.00 | Biotecnología vegetal
-81.00 | Genómica y proteómica
-82.00 | Procesos biotecnológicos
-83.00 | Técnicas instrumentales avanzadas
+departamento | total
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Educación | 3.00
+Agronomía | 1.00
+Química y Física | 2.00
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_departamento

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,10 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
+departamento | total
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Educación | 3.00
+Agronomía | 1.00
+Química y Física | 2.00
+Filología | 0.00
+Derecho | 0.00
+Biología y Geología | 0.00
```

⏱ Tiempo: 0.25 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,11 @@
-total
-12.00
+grado | total
+Grado en Ingeniería Agrícola (Plan 2015) | 0.00
+Grado en Ingeniería Eléctrica (Plan 2014) | 0.00
+Grado en Ingeniería Electrónica Industrial (Plan 2010) | 0.00
+Grado en Ingeniería Informática (Plan 2015) | 51.00
+Grado en Ingeniería Mecánica (Plan 2010) | 0.00
+Grado en Ingeniería Química Industrial (Plan 2010) | 0.00
+Grado en Biotecnología (Plan 2015) | 32.00
+Grado en Ciencias Ambientales (Plan 2009) | 0.00
+Grado en Matemáticas (Plan 2010) | 0.00
+Grado en Química (Plan 2009) | 0.00
```

⏱ Tiempo: 0.24 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,4 @@
-total
-2.00
+tipo | total_creditos
+básica | 132.00
+obligatoria | 174.00
+optativa | 180.00
```

⏱ Tiempo: 0.23 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 18: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,13 @@
-departamento | total
-Educación | 3.00
-Informática | 2.00
-Matemáticas | 2.00
-Economía y Empresa | 2.00
-Química y Física | 2.00
-Agronomía | 1.00
+nombre | apellido1 | apellido2 | total_asignaturas
+Zoe | Ramirez | Gea | 10.00
+David | Schmidt | Fisher | 0.00
+Cristina | Lemke | Rutherford | 0.00
+Esther | Spencer | Lakin | 0.00
+Carmen | Streich | Hirthe | 0.00
+Alfredo | Stiedemann | Morissette | 0.00
+Manolo | Hamill | Kozey | 11.00
+Alejandro | Kohler | Schoen | 0.00
+Antonio | Fahey | Considine | 0.00
+Guillermo | Ruecker | Upton | 0.00
+Micaela | Monahan | Murray | 0.00
+Francesca | Schowalter | Muller | 0.00
```

⏱ Tiempo: 0.28 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor, PRIMARY,id_departamento

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,2 @@
-departamento | total
-Informática | 2.00
-Matemáticas | 2.00
-Economía y Empresa | 2.00
-Educación | 3.00
-Agronomía | 1.00
-Química y Física | 2.00
-Filología | 0.00
-Derecho | 0.00
-Biología y Geología | 0.00
+nombre | apellido1 | apellido2 | fecha_nacimiento
+Pedro | Heller | Pagac | 2000-10-05
```

⏱ Tiempo: 0.22 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 20: Error
- **Descripción**: 1054 (42S22): Unknown column 'P.id_profesor' in 'on clause'

