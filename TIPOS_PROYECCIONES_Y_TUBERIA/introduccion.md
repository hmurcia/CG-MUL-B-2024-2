En computación gráfica, la representación de objetos tridimensionales en un entorno bidimensional es fundamental. Para lograr esto, se utilizan proyecciones y tuberías de visualización. Vamos a desglosar ambos conceptos.

### Tipos de Proyecciones

![image](https://github.com/user-attachments/assets/4ddbf32e-d95a-46d2-b922-ca1ef16b2e64)


Las proyecciones son técnicas que permiten representar un objeto 3D en una superficie 2D. Existen varios tipos de proyecciones, pero las más comunes son:

1. **Proyección Perspectiva**:
   - **Descripción**: Simula cómo el ojo humano ve el mundo. Los objetos que están más lejos aparecen más pequeños.
   - **Características**: Utiliza un punto de vista (cámara) desde el cual se proyectan los puntos del objeto. La proyección se basa en la intersección de líneas de visión con un plano de proyección.
   - **Usos**: Común en videojuegos y películas, donde la percepción de profundidad es crucial.

2. **Proyección Ortográfica**:
   - **Descripción**: Proyecta los puntos del objeto sin tener en cuenta la perspectiva. Las líneas paralelas permanecen paralelas en la proyección.
   - **Características**: Los objetos mantienen sus proporciones y dimensiones, independientemente de la distancia a la cámara.
   - **Usos**: Usada en diseño técnico, planos arquitectónicos y aplicaciones CAD, donde la precisión es más importante que la representación visual realista.

3. **Proyección Isométrica**:
   - **Descripción**: Un tipo específico de proyección ortográfica donde los ejes x, y, z se representan en ángulos iguales (120 grados).
   - **Características**: Permite visualizar el objeto en una vista en la que todas las dimensiones son proporcionales y no se distorsionan.
   - **Usos**: Común en videojuegos retro y gráficos de ingeniería.

### Tubería de Visualización

La tubería de visualización (o pipeline de renderizado) es el proceso a través del cual se transforman los datos 3D en una imagen 2D que se puede mostrar en pantalla. Generalmente, se divide en varias etapas:

1. **Modelado**:
   - Se crean los modelos 3D, que pueden ser generados a partir de primitivas (como cubos y esferas) o mediante técnicas más complejas como esculpido.

2. **Transformación**:
   - Se aplican transformaciones (traslaciones, rotaciones y escalados) a los modelos para situarlos en el espacio 3D. Se utilizan matrices de transformación para este propósito.

3. **Iluminación**:
   - Se calculan los efectos de la luz en los objetos. Esto implica determinar cómo las luces afectan a los materiales y cómo se proyectan las sombras.

4. **Proyección**:
   - Aquí se aplica la proyección elegida (perspectiva, ortográfica, etc.) para convertir las coordenadas 3D en coordenadas 2D.

5. **Rasterización**:
   - Los polígonos proyectados se convierten en píxeles. Este proceso determina qué píxeles de la pantalla corresponden a cada parte del objeto.

6. **Texturización**:
   - Se aplican texturas a los polígonos, mejorando el realismo visual. Esto implica mapeo UV y filtrado de texturas.

7. **Sombreado**:
   - Se aplican algoritmos de sombreado (como Gouraud o Phong) para simular cómo se ve la superficie de los objetos en función de la luz.

8. **Composición**:
   - Se combinan todas las capas y efectos (como transparencias, efectos especiales) para formar la imagen final que se presentará en pantalla.

9. **Salida**:
   - Finalmente, la imagen se muestra en el monitor. Este proceso puede incluir la optimización de la imagen para un rendimiento mejorado.

### Conclusión

Las proyecciones y la tubería de visualización son fundamentales en computación gráfica, ya que permiten transformar la complejidad de los objetos tridimensionales en imágenes comprensibles y visualmente atractivas. Cada tipo de proyección tiene sus aplicaciones específicas, mientras que la tubería de visualización es un marco integral que guía el proceso de renderizado desde el modelado hasta la visualización final.
