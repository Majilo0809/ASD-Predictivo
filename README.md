
# ASD-Predictivo

<img width="1201" height="658" alt="image" src="https://github.com/user-attachments/assets/1e6cc7c6-7c2f-4682-9335-11505032c9b9" />

# --
<img width="778" height="365" alt="image" src="https://github.com/user-attachments/assets/e8b1f8be-7322-4a5c-bf44-7ca7688e60cd" />

## --
<img width="539" height="789" alt="image" src="https://github.com/user-attachments/assets/61258909-d3fc-403f-b469-4b94fbd8cff6" />

## --
Para el cálculo de Primeros, se utilizó un algoritmo iterativo que recorre las producciones hasta que los conjuntos dejan de cambiar. Se analizan los símbolos de cada producción, agregando terminales directamente y propagando los conjuntos FIRST de los no terminales. Se maneja correctamente el símbolo ε cuando todos los símbolos de una producción pueden derivarlo.
<img width="665" height="442" alt="image" src="https://github.com/user-attachments/assets/0e8bfdf2-6d8e-4ea8-a303-9e005769f88a" />

## --
Para el cálculo de Siguientes, se aplicaron las reglas clásicas del algoritmo FOLLOW. Se inicializa el símbolo inicial con el marcador de fin de cadena ($). Luego, para cada producción, se calcula FIRST de la cadena restante (β) y se agrega al FOLLOW del símbolo correspondiente. Si β puede derivar en ε, se propaga el FOLLOW del lado izquierdo de la producción.
<img width="696" height="396" alt="image" src="https://github.com/user-attachments/assets/6e482b6d-6e9d-4076-99de-e04e84b3db9f" />


El algoritmo distingue correctamente entre terminales y no terminales, evitando errores durante la ejecución. Además, se repiten las iteraciones hasta que no se producen cambios en los conjuntos, garantizando resultados correctos.
