# Poligrafo
Este proyecto sera desarrollado con un microc-procesador del tipo DEMOQE128

Estetoscopio

Una de las partes de polígrafo está constituida por el estetoscopio permite medir  el ritmo cardíaco o pulsaciones  de la persona interroga, usando esto como uno de los parámetros para determinar si el entrevistado miente o no
Para lograr un  correcto modelaje del circuito inicialmente se procedió a simular la circuitería necesaria para su implementación como paso preliminar.

La señal es captada por un micrófono, que constituye un sensor analógico, esta se activa gracias a un divisor de voltaje en la entrada del circuito y se filtra con un capacitor de10μF para solo dejar pasar la componente AC a la entrada del bloque de ganancia

Inicialmente en el bloque de ganancia se encuentra un divisor de voltaje que determina el nivel DC a la salida del sistema. Ala entrada negativa del operacional se conecta un circuito que funciona como filtro y tiene una función similar a un circuito conversor de bipolar a unipolar, es decir deja paso solo a las componentes positivas de la salida 

Este bloque es alimentado con una fuente AC de 20mV pico y 150 Hz que corresponde a una frecuencia ubicada dentro del rango utilizado en señales bio acústicas ( 40-300 Hz)

Es importante destacar que a la salida y la entrada negativa del operacional se conecto un capacitor de  1nF.  Este limita la frecuencia a 1Khz 

f=1/(2*π*150k*1 nF)≈1000Hz
 
