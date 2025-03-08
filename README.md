# C3B
Maquina de estados finitos MSM
Desarrollo

Caja Fuerte

Ahora se procederá a realizar un contador el cual servirá para poder abrir una caja fuerte. Nuestro contador tendrá 2 botones, A y B, los cuales nos ayudarán a abrir nuestra caja con la combinación A A B. Si en el transcurso de la combinación se llegara a introducir mal algún botón, esta automáticamente regresará al estado inicial.

Tabla de estados corregida

Estado Actual

Entrada (A, B)

Estado Siguiente

Salida

S0 (00)

A = 1, B = 0

S1 (01)

0

S0 (00)

A = 0, B = 1

S0 (00)

0

S1 (01)

A = 1, B = 0

S2 (10)

0

S1 (01)

A = 0, B = 1

S0 (00)

0

S2 (10)

A = 1, B = 0

S2 (10)

0

S2 (10)

A = 0, B = 1

S3 (11)

1 (Abre caja)

S3 (11)

A = X, B = X

S0 (00)

0

Conclusión

El diseño de la máquina de estados finitos (FSM) para la caja fuerte garantiza que la secuencia de entrada correcta (A A B) desbloquee la caja, mientras que cualquier error reinicia el sistema al estado inicial. Este método proporciona una forma segura y confiable de implementar un mecanismo de acceso controlado. Además, el uso de una FSM permite una implementación eficiente con circuitos digitales en Logisim Evolution o en hardware real.
