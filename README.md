# Домаћи задатак из Техничке документације

## Задатак

Напиши програм који на основу унете дужине странице једнакостраничног троугла **a** израчунава његову површину **P**.

$\[
P = \frac{\sqrt{3}}{4} \cdot a^2
\]$

### Алгоритамска шема

```mermaid
flowchart TD
    A([START]) --> B[Unesi dužinu stranice a]
    B --> C[Izračunaj P = (√3 / 4) * a²]
    C --> D[Prikaži rezultat P]
    D --> E([END])
```

## Решење

```cs
using System;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Unesi dužinu stranice jednakoščnog trougla a:");
            double.TryParse(Console.ReadLine(), out double a);

            double P = (Math.Sqrt(3) / 4) * a * a;

            Console.WriteLine("Površina trogla iznosi " + P);
        }
    }
}
```

### Тест примери

Тест пример 1:

```text
Unesi dužinu stranice jednakoščnog trougla a:
4
Površina trogla iznosi 6,928203230275509

C:\Users\Desktop\ConsoleApp1\bin\Debug\ConsoleApp1.exe (process 13320) exited with code 0 (0x0).
Press any key to close this window . . .
```

Тест пример 2:

```text
Unesi dužinu stranice jednakoščnog trougla a:
10
Površina trogla iznosi 43,30127018922193

C:\Users\Desktop\ConsoleApp1\bin\Debug\ConsoleApp1.exe (process 15324) exited with code 0 (0x0).
Press any key to close this window . . .
```

### Објекти

| Редни број | Променљива | Тип променљиве |
| ---------- | ---------- | -------------- |
| 1.         | `a`        | `double`       |
| 2.         | `P`        | `double`       |
