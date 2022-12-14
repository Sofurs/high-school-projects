# du_1b

## Zadanie:

Zistite výsledok nasledujúcich operácií (predpokladajme, že použité premenné sú korektne deklarované) a stručne vysvetlite, prečo sa zobrazil daný výsledok.

```cpp
  int a = 3;
  int b = 2;
  std::cout << (a | b);
  std::cout << (b | a);
  std::cout << (a << b);
  std::cout << (b << a);
```

---

## Vypracovanie:

Program vytvorí premenné s názvami `a, b` a inicializuje ich na hodnoty `3, 2`. Následne sa vypíše hodnoty po operácií **or(|)**.\
Bitový posun **vľavo(<<)** posunie všetky bity o určitý počet miest.

| a | b | a \| b |
| - | - | ------ |
| 0 | 0 | 0      |
| 1 | 0 | 1      |
| 0 | 1 | 1      |
| 1 | 1 | 1      |

### a | b
```cpp
0011 == 3 
↓↓↓↓ |
0010 == 2
════	
0011 == 32
```

### b | a
```cpp
0010 == 2
↓↓↓↓ |
0011 == 3
════	
0011 == 3
```

### a << b
```cpp
3 << 2
0011 << 2
═════════
1100 == 12
```

### b << a
```cpp
2 << 3
0010 << 3
═════════
0001 0000 == 16
```

---
