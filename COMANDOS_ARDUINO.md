# Cola: Arduino / C++ — comandos essenciais

Resumo: mapeie seu pseudocódigo (VisuALG) para C++ e a estrutura Arduino (`setup()` / `loop()`).

## Estrutura mínima
```cpp
void setup() {
  Serial.begin(9600);
}

void loop() {
  // código repetitivo
}
```

## Tipos comuns
- int, long
- float, double
- bool
- String

## Serial (entrada/saída)
```
Serial.begin(9600);
Serial.print("texto");
Serial.println(valor);
if (Serial.available()) {
  int v = Serial.parseInt();
}
```

## Pinos / I/O
```
pinMode(LED_PIN, OUTPUT);
digitalWrite(LED_PIN, HIGH);
int b = digitalRead(BTN_PIN);
int val = analogRead(A0);
analogWrite(PWM_PIN, 128); // 0-255
```

## Temporização
```
delay(500); // ms — bloqueante
unsigned long t = millis(); // não bloqueante
```

## Condicionais e laços (C++ padrão)
```
if (x > 0) {
  //...
} else {
  //...
}

for (int i = 0; i < n; i++) {
  //...
}

while (cond) {
  //...
}
```

## Funções
```
int soma(int a, int b) {
  return a + b;
}
```

## Exemplo: traduzindo pseudocódigo simples
VisuALG:
```
leia(n)
se n > 10 entao
  escreva("maior")
fimse
```

Arduino/C++ equivalente (Serial):
```cpp
if (Serial.available()) {
  int n = Serial.parseInt();
  if (n > 10) {
    Serial.println("maior");
  }
}
```

## Dica rápida
- Escreva primeiro pseudocódigo claro; depois implemente `setup()` e `loop()`.
- Teste lógica via `Serial` antes de usar hardware real.

-- Fim da cola Arduino/C++ --
