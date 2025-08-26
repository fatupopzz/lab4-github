# Lab 4 - Git y GitHub Colaborativo

## Descripcion
Laboratorio colaborativo para aprender Git y GitHub, enfocado en trabajo con ramas, resolucion de conflictos y flujo de trabajo en equipo.

## Integrantes del Equipo
- **Fatima** - 24044, fanatica del kpop coreano y de la coca cola
- **Adrian Penagos** - Carne 2914, le gustan las bananas, demasiado.
- **Jose Sanchez** - Carne 24092, interesado en deportes y musica
- **Juan Gualim** - Carne 24852, le gusta pollo campero y las alitas de queso
- **Harry Mendez** - Carne 24089, le interesa la musica y ser derecho


## Estructura del Proyecto
```
lab4-github/
├── README.md
├── equipo.txt              # Archivo compartido con conflicto resuelto
├── equipo/
│   ├── fatima.md          # Informacion personal de Fatima
│   ├── adrian.md          # Informacion personal de Adrian
│   └── jose.md
|   └── juan.md            # Informacion personal de Jose
└── screenshots/           # Capturas del proceso (opcional)
```

## Proceso de Desarrollo

### Ramas Utilizadas
- **master**: Rama principal del proyecto
- **fatima-branch**: Rama de desarrollo de Fatima
- **Adrian_Pen**: Rama de desarrollo de Adrian
- **jose_branch**: Rama de desarrollo de Jose
- **gualim_branch**: Rama de desarrollo de Juan

### Workflow Implementado
1. Cada integrante trabajo en su rama personal
2. Modificaciones simultaneas del archivo compartido equipo.txt
3. Integracion paso a paso mediante merge a master
4. Resolucion manual de conflictos detectados

## Conflicto Resuelto

### Descripcion del Conflicto
- **Archivo afectado**: equipo.txt
- **Ramas en conflicto**: Adrian_Pen vs jose_branch  
- **Causa**: Ambas ramas modificaron completamente el contenido del archivo
- **Tipo**: Conflicto de contenido total

### Contenido Original en Conflicto

**Rama Adrian_Pen contenia:**
```
Mi nombre es Adrian Penagos, mi numero de carne es 2914.
Me gustan mucho las bananas, los videojuegos y dibujar.
Quiero dedicarme al UI / UX design
```

**Rama jose_branch contenia:**
```
Hola, soy Jose Sanchez y mi carnet es 24092.
Me gustan los deportes y la musica.
```

### Proceso de Resolucion
1. **Deteccion**: Git identifico automaticamente el conflicto durante el merge
2. **Analisis**: Revision del contenido conflictivo usando git status y cat equipo.txt
3. **Edicion manual**: Combinacion de ambas contribuciones en un formato unificado
4. **Validacion**: Verificacion de que toda la informacion fue preservada
5. **Finalizacion**: Commit de la resolucion y push al repositorio

<img width="1398" height="670" alt="image" src="https://github.com/user-attachments/assets/97f46379-7130-4df7-a6a3-b9c034d89e91" />


### Solucion Implementada
```
=== PRESENTACIONES DEL EQUIPO LAB4 ===

Adrian Penagos - Carne: 2914
Me gustan mucho las bananas, los videojuegos y dibujar.
Quiero dedicarme al UI / UX design

Jose Sanchez - Carne: 24092  
Me gustan los deportes y la musica.

=== CONFLICTO RESUELTO EXITOSAMENTE ===
```

## Comandos Git Utilizados

### Configuracion inicial
```bash
git init
git remote add origin [URL]
git clone [URL]
git config --global user.name "nombre"
git config --global user.email "email"
```

### Trabajo con ramas
```bash
git branch                    # Listar ramas locales
git branch -a                 # Listar todas las ramas
git checkout [rama]           # Cambiar de rama
git checkout -b [nueva-rama]  # Crear y cambiar a nueva rama
git merge [rama]              # Fusionar rama
```

### Sincronizacion con repositorio remoto
```bash
git fetch origin             # Actualizar referencias remotas
git fetch origin --all       # Actualizar todas las ramas remotas
git pull origin [rama]       # Actualizar rama local con remota
git push origin [rama]       # Subir cambios al repositorio remoto
```

### Resolucion de conflictos
```bash
git status                   # Ver estado del conflicto
cat [archivo]               # Inspeccionar contenido conflictivo
[edicion manual del archivo]
git add [archivo]           # Marcar conflicto como resuelto
git commit -m "mensaje"     # Confirmar resolucion
git push origin master      # Subir resolucion al repositorio
```

### Historial y seguimiento
```bash
git log --oneline           # Ver historial resumido
git log --graph             # Ver historial con ramas graficamente
git diff [rama1] [rama2]    # Comparar diferencias entre ramas
git blame [archivo]         # Ver quien modifico cada linea
```

## Aprendizajes del Laboratorio

### Aspectos Colaborativos
- **Comunicacion en equipo**: Fundamental para coordinar cambios y evitar conflictos innecesarios
- **Distribucion de trabajo**: Cada miembro puede trabajar independientemente en su rama
- **Revision de codigo**: Importante validar cambios antes de integrar
- **Documentacion**: Mensajes de commit descriptivos ayudan a entender el proceso


## Reflexion del Equipo

### Areas de Mejora
- Planificacion previa para minimizar conflictos
- Coordinacion mas estrecha en modificaciones de archivos compartidos
- Implementacion de revision de codigo antes del merge
- Uso de pull requests para mejorar el flujo de trabajo

### Aplicaciones Futuras
- Implementar este flujo en proyectos de desarrollo reales
- Utilizar ramas de feature para desarrollo de nuevas funcionalidades
- Aplicar mejores practicas de commit y documentacion
- Coordinar trabajo en equipo usando herramientas colaborativas

## Resultados del Laboratorio

**Estado final del proyecto:**
- Conflicto detectado automaticamente por Git
- Resolucion exitosa preservando todas las contribuciones  
- Integracion completa de información de los tres miembros
- Documentacion exhaustiva del proceso de resolucion
- Aprendizaje practico de herramientas de control de versiones

**Archivos finales integrados:**
- equipo.txt: Presentaciones completas del equipo con conflicto resuelto
- Archivos individuales: Informacion personal de cada miembro
- Documentacion: README.md con proceso completo documentado

---
<img width="2258" height="906" alt="image" src="https://github.com/user-attachments/assets/f5e3b7c0-8c01-4fde-b389-fabba0f94f9e" />

**Laboratorio completado exitosamente**

**Responsable de resolucion:** Fatima  
**Colaboradores:** Adrian Penagos, Jose Sanchez, Gualim, Daniel y Harry  
**Objetivo alcanzado:** Comprension practica de resolucion de conflictos en Git

<img width="2272" height="632" alt="image" src="https://github.com/user-attachments/assets/5392d7ff-d35d-4df7-b99f-0977e78517a2" />

