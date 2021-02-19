Repozytorium zawiera projekt zaliczeniowy z przedmiotu "Algorytmy Ewolucyjne".
Polegał on na zastosowaniu różnych podejść, aby wygenerować obraz przypominający MonaLisę za pomocą ograniczonej liczby kół.
Szczegółowy opis problemu, zastosowanych algorytmów i uzyskanych wyników można znaleźć w pliku "Raport".

## Jak uruchomić plik?

Polecam uruchamianie notatników w Colabie (colab.research.google.com).
Proszę zwrocić uwagę na to, aby biblioteka Pillow była w wersji 8.
W przeciwnym wypadku, obwód koła będzie ciemniejszy niż jego wypełnienie.
Aby zaktualizować Pillowa, trzeba wykonać pierwszy blok kodu zawarty w każdym z notebooków:
```
!pip install --upgrade Pillow
pass
```
Najczęściej będzie po tym trzeba zrestartować środowisko uruchomieniowe.
Następnie należy pobrać obrazek:
<img src="https://i.imgur.com/fc2ASJh.png" alt="">
Powinien on mieć wymiary 299 x 299 px.
Należy go nazwać ‘monalisa.jpg’ i umieścić na swoim Dysku Google, a następnie przesłać go do Colaba wykonując kolejne bloki kodu.
Oczywiście możliwe jest wykorzystanie innych obrazków, ale rozmiar 299 x 299 jest zahardcode’owany w paru miejscach i należałoby go wtedy zmienić.

## Jak zapewniana jest powtarzalność wyników?
Przed każdym uruchomieniem algorytmu, ziarno losowości jest ustawiane na 0.
```
random.seed(0)
np.random.seed(0)
```

## Mapowanie metoda-nazwa pliku:

1. Metoda 1:
 - bez ogarniczeń na liczbę kół: MonaLisaM1.ipynb
 - ścisły limit na liczbę kół: MonaLisaM1:twardy_limit.ipynb
 - większy minimalny rozmiar koła: MonaLisaM1:wieksze_kola.ipynb
 - funkcja celu karająca koła ponad limit: MonaLisaM1:funkcja_celu_karajaca_kola.ipynb
 - mniejsze prawdopodobieństwo dodania koła ponad limit przez mutację: MonaLisaM1:mutacja_zalezna_od_kol.ipynb
2. Metoda 2: MonaLisaM2.ipynb

## Link do archiwum większej niż w raporcie liczby wyników pośrednich
Większą liczbę wyników pośrednich można znaleźc pod linkiem:
https://hackmd.io/@f_3wnjZLTny2wfs_633y1g/HkSI8CR1O
