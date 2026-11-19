# Nombre del proyecto



# Descripción del problema



# Pregunta de investigación
¿Qué tan grande puede ser el paso de tiempo (Δt) en la integración de Euler antes de que un proyectil rápido atraviese una pared delgada de grosor e sin que la simulación detecte el impacto (tunneling)?


# Modelo físico
Proyectil como partícula puntual en 2D, lanzada desde el origen con rapidez v₀ y ángulo θ contra una pared vertical de grosor e situada en x = x_b. Con la segunda ley de Newton (ΣF = ma) considerando solo el peso:

	•	Eje x: aₓ = 0 → vₓ(t) = v₀·cos(θ) (constante)
	•	Eje y: a_y = -g → v_y(t) = v₀·sen(θ) - g·t

Suposiciones: g = 9.8 m/s² constante, sin resistencia del aire, sin rotación y pared rígida e inmóvil.


# Métodos numéricos utilizados
Método de Euler escrito por nosotros en Python (NumPy y Matplotlib). La colisión se evaluará de forma discreta, verificando en cada paso si x_b ≤ xₙ ≤ x_b + e. Haremos un barrido de Δt (de 10⁻⁴ s a 10⁻¹ s) para identificar el umbral en el que el proyectil "salta" la pared sin activar la condición de choque.


Cómo instalar dependencias y ejecutar el proyecto.



Resultados y conclusiones.



Integrantes
Julian
Maria Alejandra Sanabria Salazar