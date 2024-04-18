# Responzivní webdesign

Pojem vymyslel __*Ethan Marcotte*__ ve své knize **Responsive Web Design**.

Cílem je zajistit optimální uživatelskou přístupnost na mnoha různých zařízeních.

Stránka se přizpůsobuje - upravuje svoje rozložení a obsah podle prostředí, ve kterém je prohlížena.

<br/><br/><br/><br/><br/>

## Přístupy

### ~~DESKTOP FIRST~~

Výchozí je rozložení pro desktop. Až potom vytváříme design pro tablet a mobil.

### MOBILE FIRST

Výchozí je rozložení pro mobily. Postupně přidáváme prvky pro tablety a osobní počítače.


<br/><br/>

## Základní techniky

1. Responzivní meta tag
1. Rozměry v relativních jednotkách (procenta, ale i třeba *vw* nebo *vh*)
1. Media queries (dotazy na médium)



<br/><br/><br/><br/><br/><br/>

## Media query
Také **dotaz na médium**.

<br/>

```css
@media (min-width: 800px) {
    p {
        color: black;
    }
}
```
<br/><br/><br/>

#### Další příklady

Pro tiskárnu:
```css
@media print {
    body {
        font-size: 10pt; 
    }
}
```
Pro obrazovku:
```css
@media screen {
    body {
        font-size: 13px;
    }
}
```
Pro obojí:
```css
@media screen, print {
    body {
        line-height: 1.2; 
    }
}
```
<br/><br/><br/><br/><br/><br/>
#### Kombinace

```css
@media screen and (min-width: 900px) {
    article {
        padding: 1rem 3rem;
    }
}
```

```css
@media screen and (min-width: 320px) and (max-width: 480px) and (resolution: 150dpi) {
    body {
        line-height: 1.4;
    }
}
```

<br/><br/><br/><br/><br/><br/>

Další info zde:
https://www.vzhurudolu.cz/prirucka/css3-media-queries

<br/><br/><br/>