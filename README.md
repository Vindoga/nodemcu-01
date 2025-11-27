# Lärdomar från vecka 3 #
## NodeMCU
Vad är en NodeMCU? Det är ett litet och billigt mikrokontrollerkort baserat på ESP8266 eller ESP32. Det används för att bygga enkla IoT-projekt (Internet of Things).
Ett sådant projekt kan exempelvis vara en sensor av något slag (temperatur, ljus, ljud, vikt, etc).

## Hur börjar man?
1. Installera Arduino IDE
2. Lägg till stödet ESP8266 eller ESP32 i Arduino
3. Anslut USB till din NodeMCU
4. Börja experimentera

## Exempelkod
Här är ett exempel på hur en kod kan skrivas för att tända en LED lampa en sekund och stänga av en sekund, upprepningsvis:
```
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

## Vad är Arduino IDE?
Det är mjukvaruprogrammet man använder för att skriva och ladda upp kod för NodeMCU. Programmet kommer med diverse fördelar såsom att det är enkelt att lära sig. I text editorn skriver man sin kod i C++ språk.
Sen trycker man på compile/verify och då letar Arduino efter fel med koden och ger förslag på vad som borde justeras. Sen finns det ett stort bibliotek med färdigskriven kod redo att klistras in.

## Mikroprocessor
