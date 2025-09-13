# Guía para Instructores - Git Learning Exercises

Esta guí## Evaluación
- Ejercicios 1-2: Fundamentos (0.25 puntos)
- Ejercicios 3-4: Intermedio (0.35 puntos)  
- Ejercicios 5-7: Avanzado (0.4 puntos)

¡Buena suerte!yudará a configurar y utilizar este repositorio de ejercicios de Git con GitHub Classroom.

## 🎯 Configuración Inicial

### 1. Preparar el Repositorio Template

1. **Fork o usa este repositorio** como template en tu organización de GitHub
2. **Asegúrate de que todos los archivos están presentes**:
   - Ejercicios 6-12 en la carpeta `ejercicios/`
   - Tests correspondientes en `tests/ejercicio/`
   - Configuración de autograding en `.github/`

### 2. Configurar GitHub Classroom

1. **Ve a [GitHub Classroom](https://classroom.github.com/)**
2. **Crea una nueva asignación (Assignment)**
3. **Configura los siguientes parámetros**:
   - **Template repository**: Tu fork de este proyecto
   - **Assignment title**: "Git Learning Exercises"
   - **Assignment description**: Ver ejemplo abajo
   - **Deadline**: Según tu cronograma
   - **Enable autograding**: ✅ Activado

### 3. Configurar Autograding

En GitHub Classroom, configura los siguientes tests de autograding:

| Test Name | Setup Command | Run Command | Timeout | Points |
|-----------|---------------|-------------|---------|--------|
| Git Initialization | `npm install` | `npm test ejercicio/1` | 10s | 0.1 |
| First Commit | - | `npm test ejercicio/2` | 10s | 0.15 |
| Multiple Commits | - | `npm test ejercicio/3` | 10s | 0.15 |
| Branches | - | `npm test ejercicio/4` | 15s | 0.2 |
| GitHub Integration | - | `npm test ejercicio/5` | 15s | 0.2 |
| Pull and Clone | - | `npm test ejercicio/6` | 10s | 0.1 |
| Conflict Resolution | - | `npm test ejercicio/7` | 15s | 0.1 |

**Total de puntos**: 1.0

## 📝 Descripción de Asignación Sugerida

```markdown
# Ejercicios de Git - Aprendizaje Progresivo

## Objetivos
Al completar esta asignación, serás capaz de:
- Inicializar y configurar repositorios Git
- Realizar commits y gestionar cambios
- Trabajar con ramas y fusiones
- Integrar Git con GitHub
- Resolver conflictos de merge

## Instrucciones
1. Acepta esta asignación y clona tu repositorio
2. Instala las dependencias: `npm install`
3. Completa los ejercicios del 6 al 12 en orden
4. Ejecuta los tests para verificar tu progreso: `npm test ejercicio/X`
5. Haz push de todos tus cambios

## Evaluación
- Ejercicios 6-7: Fundamentos (25 puntos)
- Ejercicios 8-9: Intermedio (35 puntos)  
- Ejercicios 10-12: Avanzado (40 puntos)

¡Buena suerte!
```

## 🏗️ Estructura Pedagógica

### Progresión de Dificultad

**Nivel Básico (Ejercicios 1-2)**: 
- Configuración inicial
- Conceptos fundamentales
- Primer contacto con Git

**Nivel Intermedio (Ejercicios 3-4)**:
- Flujos de trabajo más complejos
- Gestión de ramas
- Conceptos de merge

**Nivel Avanzado (Ejercicios 5-7)**:
- Integración con GitHub
- Trabajo colaborativo
- Resolución de conflictos

### Tiempo Estimado

- **Por ejercicio**: 15-30 minutos
- **Total**: 2-3 horas
- **Recomendado**: Distribuir en 2-3 sesiones

## 📊 Monitoreo del Progreso

### Dashboard de GitHub Classroom

GitHub Classroom proporciona:
- **Vista general del progreso** de todos los estudiantes
- **Resultados de autograding** en tiempo real
- **Estadísticas de commits** y actividad
- **Identificación de estudiantes** que necesitan ayuda

### Señales de Alerta

Presta atención a estudiantes que:
- No tienen commits después de 1 semana
- Fallan consistentemente los tests básicos
- No siguen la progresión esperada

## 🔧 Personalización

### Modificar Ejercicios

Para adaptar los ejercicios a tu contexto:

1. **Edita los archivos markdown** en `ejercicios/`
2. **Actualiza los tests correspondientes** en `tests/ejercicio/`
3. **Ajusta los criterios de evaluación** si es necesario

### Añadir Ejercicios

Para añadir nuevos ejercicios:

1. Crea `ejercicios/ejercicio-X-nombre.md`
2. Crea `tests/ejercicio/X-nombre.test.js`
3. Actualiza el autograding configuration

## 🆘 Problemas Comunes

### Estudiantes No Pueden Instalar Dependencias

**Solución**: Proporciona instrucciones para:
- Instalar Node.js v16+ 
- Verificar npm está funcionando
- Usar `npm install --legacy-peer-deps` si es necesario

### Tests Fallan por Configuración de Git

**Solución**: Los estudiantes necesitan:
```bash
git config --global user.name "Su Nombre"
git config --global user.email "su.email@ejemplo.com"
```

### Conflictos con Ramas Principales

Algunos repositorios usan `master`, otros `main`:
- Los tests están diseñados para aceptar ambos
- Instruye a los estudiantes sobre su configuración específica

### Autograding No Funciona

Verifica que:
- El repositorio template tiene `.github/workflows/` y `.github/classroom/`
- Los tests pasan en el repositorio template
- Las dependencias están correctamente especificadas

## 📈 Métricas de Éxito

### Indicadores Cuantitativos

- **Tasa de completación**: >80% completan al menos 5 ejercicios
- **Tasa de éxito**: >70% obtienen al menos 0.7 puntos
- **Tiempo promedio**: 2-4 horas para completar todo

### Indicadores Cualitativos

- Estudiantes usan Git en proyectos posteriores
- Mejor comprensión de workflows de desarrollo
- Mayor confianza en herramientas de control de versiones

## 🤝 Soporte a Estudiantes

### FAQ Común

**P: ¿Por qué fallan mis tests si seguí las instrucciones?**
R: Verifica que hayas hecho commit de todos los cambios y que no tengas archivos sin trackear.

**P: ¿Puedo usar GitHub Desktop en lugar de línea de comandos?**
R: Los ejercicios están diseñados para línea de comandos, pero GitHub Desktop puede complementar el aprendizaje.

**P: ¿Qué hago si rompo mi repositorio?**
R: Puedes clonarlo nuevamente o usar `git reset` para volver a un estado anterior.

### Recursos Adicionales para Estudiantes

- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Interactive Git Tutorial](https://learngitbranching.js.org/)
- [GitHub Learning Lab](https://lab.github.com/)

---

## 💡 Consejos para el Éxito

1. **Haz una demostración en vivo** de los primeros ejercicios
2. **Programa sesiones de ayuda** para estudiantes con dificultades
3. **Fomenta la colaboración** entre estudiantes para resolver problemas
4. **Conecta con proyectos reales** para mostrar la aplicación práctica
5. **Celebra los logros** cuando los estudiantes completan ejercicios difíciles

¡Esperamos que estos ejercicios ayuden a tus estudiantes a dominar Git! 🚀
