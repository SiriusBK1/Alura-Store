~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~ .oooooo..o  o8o            o8o                          oooooooooo.  oooo       ~
~d8P'    `Y8  `"'            `"'                          `888'   `Y8b `888       ~
~Y88bo.      oooo  oooo d8b oooo  oooo  oooo   .oooo.o     888     888  888  oooo ~
~ `"Y8888o.  `888  `888""8P `888  `888  `888  d88(  "8     888oooo888'  888 .8P'  ~
~     `"Y88b  888   888      888   888   888  `"Y88b.      888    `88b  888888.   ~
~oo     .d8P  888   888      888   888   888  o.  )88b     888    .88P  888 `88b. ~
~8""88888P'  o888o d888b    o888o  `V88V"V8P' 8""888P'    o888bood8P'  o888o o888o~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

# Análisis de Tiendas – Decisión de Venta del Sr. Juan

Proyecto de análisis de datos de ventas de cuatro tiendas para determinar cuál presenta **peor desempeño** y debería ser vendida.  
Desarrollado por Adrián | Branding: SiriusBk  

---

## Objetivo  
Identificar la tienda con **indicadores más bajos** (ingresos, rotación de productos, reseñas y costos de envío) para recomendar su venta.  

---

## Metodología  

### 1. **Carga y Preparación de Datos**  
- Lectura de datos desde archivos CSV de cada tienda.  
- Integración de un campo `tienda` para identificar el origen.  
- Concatenación de todos los registros en un único DataFrame.  
- Análisis de métricas clave: ingresos, calificaciones, envío, productos más y menos vendidos.

### 2. **Análisis Exploratorio**  
- Cálculo de **ingresos totales por tienda**.  
- Evaluación de **reseñas promedio por tienda**.  
- Determinación del **costo de envío promedio**.  
- Identificación de **categorías y productos más y menos vendidos**.  
- Generación de gráficos:  
  - Barras (ingresos por tienda).  
  - Barras y dispersión (productos menos vendidos por tienda).  
  - Circular o barras (distribución de categorías).  

---

## Principales Hallazgos  

### Ingresos Totales
- **Tienda 4** presenta los ingresos más bajos (≈1.038 millones), mientras que Tienda 1 es la más rentable (≈1.151 millones).

### Reseñas Promedio
- Todas las tiendas tienen calificaciones similares (~4), sin compensar las diferencias en ingresos y ventas.

### Costo de Envío Promedio
- Tienda 4 tiene el **menor costo de envío**, aunque esto no compensa su bajo desempeño en ventas.

### Productos y Categorías
- **Productos más vendidos**: Mesa de noche, Carrito de control remoto, Microondas, Batería, Cama king.  
- **Productos menos vendidos**: Concentración mayor en Tienda 4.  
- **Categorías más vendidas**: Muebles, Electrónicos, Juguetes, Electrodomésticos, Deportes y diversión.  

---

## Conclusión y Recomendación

Con base en el análisis:

- **Peor desempeño global**: Tienda 4 (menores ingresos y concentración de productos de baja rotación).  
- **Recomendación**: El Sr. Juan debería **vender Tienda 4**, optimizando así la operación y concentrándose en tiendas más rentables.

---

## Próximos Pasos

1. Analizar el **ranking de productos menos vendidos por tienda** para confirmar la proporción de baja rotación.  
2. Evaluar la **sensibilidad de margen** relacionada con el menor costo de envío.  
3. Simular el impacto de **cerrar Tienda 4** en la mezcla de categorías y cobertura geográfica.  

---

## Tecnologías Utilizadas
- Python: pandas, numpy, matplotlib.  
- Herramientas: Google Colab, Jupyter Notebook.  

---

## Cómo Reproducir

```bash
git clone https://github.com/SiriusBK1/Challenge-Tiendas
pip install -r requirements.txt  # pandas, matplotlib, numpy
jupyter notebook Analisis_Tiendas.ipynb

👤 Autor

Adrián — Estudiante de Data Science
🔗 GitHub: SiriusBk
📬 Contacto: aacevedovergara@gmail.com
