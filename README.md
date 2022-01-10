# PRiR zadania lab 10
Całkowanie numeryczne metodą prostokątów, trapezów oraz Simpsona.<br>
Wzór funkcji do całkowania: f(x) = x^2 + 2x + 13 <br> 
Przedziały całkowania: (-3, 7)<br>
Wersja CPU:
```
prostokat dla n1 = 100000: 0.00153000, 293.335999
prostokat dla n2 = 1000000: 0.01521500, 293.325714
prostokat dla n3 = 10000000: 0.15084500, 287.964722
trapez dla n1 = 100000: 0.00131300, 293.332794
trapez dla n2 = 1000000: 0.01432000, 293.347443
trapez dla n3 = 10000000: 0.13275100, 290.808258
simpson dla n1 = 100000: 0.00247000, 293.332794
simpson dla n2 = 1000000: 0.02473100, 293.347473
simpson dla n3 = 10000000: 0.24791900, 290.808258
```

Wersja GPU:
```
prostokat dla n1 = 100000: 0.129686, 293.328
prostokat dla n2 = 1000000: 0.00961065, 293.325
prostokat dla n3 = 10000000: 0.0923725, 287.965
trapez dla n1 = 100000: 0.0060568, 293.333
trapez dla n2 = 1000000: 0.00792065, 293.347
trapez dla n3 = 10000000: 0.0770713, 290.808
simpson dla n1 = 100000: 0.00760585, 293.335
simpson dla n2 = 1000000: 0.0238274, 293.348
simpson dla n3 = 10000000: 0.0202489, 293.348
```
![](mProstokat.png)<br><br>
![](mTrapez.png)<br><br>
![](mSimpson.png)
Wnioski: Im większe n, tym wydajniejsza jest wersja GPU algorytmów. Dla mniejszych n CPU okażę się być szybsze ze względu na to, że w wersji GPU dużo czasu zajmuje kopiowanie danych między CPU a GPU.
