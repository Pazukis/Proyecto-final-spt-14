# sql-bookstore-data-analysis

## Objetivo General

Analizar una base de datos de una aplicación de lectura para generar una propuesta de valor basada en:
- Publicaciones recientes
- Editoriales y autores destacados
- Calificaciones y reseñas de usuarios

---

## Tareas Descompuestas

### 1. Conexión y Exploración Inicial
- [ ] Conectarse a la base de datos proporcionada
- [ ] Visualizar las primeras filas de cada tabla (`books`, `authors`, `publishers`, `ratings`, `reviews`)
- [ ] Verificar tipos de datos y relaciones clave

---

### 2. Consultas SQL Específicas

#### 2.1 Libros publicados después del 1 de enero de 2000
- [ ] Escribir consulta SQL para contar libros con `publication_date > '2000-01-01'`
- [ ] Mostrar resultado y describir hallazgos

#### 2.2 Número de reseñas y calificación promedio por libro
- [ ] Unir `ratings` y `reviews` por `book_id`
- [ ] Agrupar por libro y calcular:
  - Número de reseñas
  - Calificación promedio

#### 2.3 Editorial con más libros de más de 50 páginas
- [ ] Filtrar libros con `num_pages > 50`
- [ ] Agrupar por `publisher_id` y contar
- [ ] Unir con `publishers` para obtener el nombre

#### 2.4 Autor con la calificación promedio más alta (mínimo 50 calificaciones)
- [ ] Agrupar `ratings` por `book_id`, contar y promediar
- [ ] Filtrar libros con al menos 50 calificaciones
- [ ] Unir con `books` y `authors` para obtener el autor

#### 2.5 Número promedio de reseñas de texto entre usuarios que calificaron más de 50 libros
- [ ] Contar calificaciones por `username` y filtrar usuarios con más de 50
- [ ] Contar reseñas de texto por esos usuarios
- [ ] Calcular promedio

---

## Consideraciones Técnicas
- Todas las consultas deben realizarse con SQL
- Usar `pandas` solo para mostrar y almacenar resultados
- Documentar cada paso con conclusiones claras

---

## 📫 Contacto del Autor

Paz Emmanuel Balderas Cerezo  
📧 pazemmanuel24032005@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/paz-emmanuel-balderas-cerezo-dataanalyst)
