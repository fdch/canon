# Canon

## Program Notes

"Canon" aims to reflect on the concept of a canon, both in its definition as rule, and as musical genre. All players are in canon, but this canon can never be heard. This work is an exploration of noise in society, and a question regarding the process of music composition as a canon in itself. It was composed for and premiered by Proyecto[Red]Ensamble at Centro Cultural Graciela Carena, CBA, ARG, in August 2016.

## Aditional Notes

All players have one instrument and one potentiometer. The players follow the score performing both with their potentiometer and with their instrument. The data obtained from the potentiometers is then interpreted as the speed at which a [lorenz] system is iterated (which is between 0.001 and 1 every sample, at a given samplerate, e.g 44100 Hz). The output (X,Y,Z) from each system is interpreted in two ways: first, it is read as a signal and added altogether; second, it is parsed through [siginfo] to obtain slope changes, which are as well read as signals and added altogether. Finally, the distance obtained from [siginfo] serves as gain for the final signal. One player can be given a midi input to trigger randomized variables for all (or each) lorenz system(s), generating divergence among the randomized systems. Within this midi input, one note (MIDI Note 72) serves as on/off switch for the patch. A timer is provided on the screen. The whole work lasts at least 6 minutes, but the duration bends when there are CPU overloads. It is encouraged to "surf" in and out of those CPU overloads by simply changing the potentiometer to a value closer to 1, or to 0 in case there is a need to stop all iterations from the potentiometer involved.

## Performance Instructions 

(In spanish for now...)

1. Conectar teclado midi (usb) y placa de sonido primero
2. Abrir PD (vanilla, version 0.47-1)
3. Abrir main.pd
4. DSP tiene que estar encendido == Patch esta listo
5. Midi nota 72 EMPIEZA (se vuelve verde)
5. (apretar el boton "start" verde para que inicie el cronometro)
5. (cuidado que "reset", boton naranja, reinicia el cronometro... y "stop", boton rojo, lo apaga....)
5. APRETAR libremente "diverge", boton amarillo, cada tanto...
6. Midi nota 72 TERMINA (se vuelve rojo) <-- NO APRETAR MAS DE UNA VEZ... Tiene un retraso de 10 segundos, pero va a andar (va a hacer un fade-out que es necesario para el final de la obra)

### NOTA:

Midi notas 48 50 52 53 55 (DO-RE-MI-FA-SOL) hacen que los sistemas de lorenz tengan distintas condiciones iniciales, y entonces divergen entre si, APRETARLAS


Las teclas midi tambien hacen sonidos, asi que tocalas!!

salutes!

fch226@nyu.edu