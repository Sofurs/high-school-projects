# du_1a

## Zadanie:

Zistite výsledok nasledujúcich operácií (predpokladajme, že použité premenné sú korektne deklarované) a stručne vysvetlite, prečo sa zobrazil daný výsledok.

```cpp
  int cislo = 172;
  cislo &= 3;
  std::cout << cislo;
```

---

## Vypracovanie:

Program vytvorí premennú s názvom `cislo` a inicializuje ju na hodnotu `172`, ku ktorej sa pomocou bitovej operácie **and(&)** pridá hodnota `3`.

| a | b | a & b |
| - | - | ----- |
| 0 | 0 | 0     |
| 1 | 0 | 0     |
| 0 | 1 | 0     |
| 1 | 1 | 1     |

```cpp
1010 1100 == 172
↓↓↓↓ ↓↓↓↓ &
0000 0011 == 3
═════════	
0000 0000 == 0
```

---
