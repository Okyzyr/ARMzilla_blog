---
title: "ARMzilla - Początek"
date: 2025-07-20
draft: false
tags: ["armzilla", "arm", "projekty"]
---


# Wprowadzenie

Projekt ARMzilla to próba samodzielnego zaprojektowania i zbudowania niewielkiego robotycznego ramienia inspirowanego rozwiązaniami przemysłowymi. Jego głównym celem jest praktyczna nauka — od podstaw — zagadnień związanych z kinematyką, elektroniką i programowaniem.

Projekt zakłada stopniowe zdobywanie wiedzy i umiejętności w zakresie:
- obliczania sił i momentów (kinematyka i statyka),
- doboru i sterowania silnikami krokowymi,
- nauki korzystania z Autodesk Fusion oraz projektowania mechanicznego,
- tworzenia elektroniki sterującej,
- programowania mikrokontrolerów.

Wszystkie elementy projektu mają być w pełni autorskie. Najważniejszym aspektem całego przedsięwzięcia będzie samodzielne rozwiązywanie problemów pojawiających się na kolejnych etapach rozwoju — od pierwszego szkicu, aż po działający prototyp.

## Inspiracje

Inspiracją do rozpoczęcia projektu były przykłady prostych, ale przemyślanych konstrukcji robotycznych, które można znaleźć w sieci. Na początku zbudowałem ramię MeArm 0.4, ale od razu poczułem, że można mierzyć wyżej. 
Niektóre z tych nagrań pokazują, że nawet przy ograniczonym budżecie i dostępnych narzędziach da się zbudować funkcjonalne i dobrze działające ramię robotyczne.

Dwa konkretne materiały, które ogólnie pokazują zasadę działania takiego urządzenia:


<iframe width="100%" height="315" src="https://www.youtube.com/embed/EN3Op92fBaE" frameborder="0" allowfullscreen></iframe>


- [https://www.youtube.com/shorts/EN3Op92fBaE](https://www.youtube.com/shorts/EN3Op92fBaE) – krótka prezentacja bardzo czystego i solidnie wyglądającego ramienia opartego na silnikach krokowych z przekładniami. Podoba mi się w nim zwartość konstrukcji, budowa i ogólna estetyka wykonania.

<iframe width="100%" height="315" src="https://www.youtube.com/embed/tJFFxlo26fk" frameborder="0" allowfullscreen></iframe>

- [https://youtu.be/tJFFxlo26fk](https://youtu.be/tJFFxlo26fk) – dłuższy materiał prezentujący złożony projekt, w którym widać cały cykl pracy: projektowanie, druk, montaż i testowanie. Choć to ramię wygląda na bardziej rozbudowane niż to, co planuję w pierwszej wersji, pokazuje dobre praktyki i daje wyobrażenie o kolejnych etapach rozwoju.

Oba filmy pokazały mi, że warto spróbować — nawet jeśli na początku brakuje doświadczenia, można dużo osiągnąć dzięki systematycznej pracy i nauce na własnych błędach.

## Założenia techniczne

- Napęd: silniki krokowe NEMA 17 i NEMA 23 z przekładniami
- Konstrukcja:  
  - ramię ma się składać z 4 silników i jednego serwomechanizmu. 
  - budowę podzieliłem na kilka cześci:
    - "podstawa" - obrotowa
    - "ramię" - podnosi całość
    - "łokieć" - podnosi i opuszcza dłoń
    - "dłoń" - obrotowa, zakończona serwomechanizmem
  - wersja prototypowa: druk 3D  
  - wersja docelowa: frezowane aluminium (jeśli będzie to możliwe)
- Sterowanie: ESP32 DevKit lub Raspberry Pi
- Język programowania: C++ lub Python (ostateczny wybór zapadnie w trakcie prac)


## Zastrzeżenie

W trakcie realizacji projektu mogą (i zapewne będą) pojawiać się błędy: w obliczeniach, konstrukcji, doborze części lub założeniach niezgodnych z rzeczywistością. Ten projekt ma jednak służyć przede wszystkim nauce — także na własnych pomyłkach. Wpisy będą odzwierciedlały rzeczywisty przebieg prac, bez upiększania. Jednak zaznaczam, że nie znajdziecie tutaj właściwego technicznego języka czy systemu pracy do którego pewnie każdy student politechniki jest przyzwyczajony. 

## Cel bloga

Ten blog ma służyć jako dokumentacja całego procesu — od pierwszych założeń po finalny efekt. Będą się tu pojawiać notatki techniczne, analizy, decyzje projektowe oraz napotkane problemy i sposoby ich rozwiązania.

Wszystkie pliki i projekty będą publikowane na otwartej licencji — szczegóły zostaną udostępnione w repozytorium.
