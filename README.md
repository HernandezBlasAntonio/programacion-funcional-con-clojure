# Programación Funcional con Clojure

- [Introducción](#introducción)
   - [Mí intención](#mí-intención)
   - [Lo que busco...](#lo-que-busco)
   - [Lo que no busco...](#lo-que-no-busco)
   - [Lo que te recomiendo...](#lo-que-te-recomiendo)
- [Sobre Clojure](#sobre-clojure)
- [Entorno de trabajo](#entorno-de-trabajo)
- [Course Design Philosophy](#course-design-philosophy)
- [Créditos](#créditos)
- [Copyright and License](#copyright-and-license)

# Introducción

Este taller busca familiarizarnos a razonar de manera _funcional_, usando el lenguaje de
programación [Clojure](https://clojure.org) como _herramienta_ de razonamiento.

## Mí intención

Dos frases que nos sirven de contexto, una por parte de
[Alan J. Perlis](http://pu.inf.uni-tuebingen.de/users/klaeren/epigrams.html):

> Un lenguaje que no afecta tu forma de pensar en la programación, no merece ser aprendido.

De tal forma que la intención es exponernos a un lenguaje de programación y aprender algunas de
sus características que pueden afectar nuestra manera de analizar y resolver problemas.

Y la otra frase por [Uriel](https://docs.huihoo.com/plan9/Plan9.pdf):
> Para realmente comprender a Plan 9, tienes que **des-aprender** los últimos 30 años de Unix.
> Las similitudes son lo suficientemente grandes como para crear falsas expectativas.

Basta con hacer unos ajustes para obtener lo siguiente:

> Para realmente comprender a la Programación Funcional, tienes que **des-aprender** los últimos
> 30 años de Programación Imperativa/Orientada a Objetos. Las similitudes son lo suficientemente
> grandes como para crear falsas expectativas.

## Lo que busco

  - Familiarizarnos con el lenguaje de programación Clojure, tanto en su sintaxis y semántica.
  - Familiarizarnos con _"ideas avanzadas"_ en programación a partir de elementos _primitivos_
    en Clojure.
     - Ideas tales como: _inmutabilidad_, _estructuras de datos inmutables_, _recursividad_,
       _evaluación perezosa_, _aridad de funciones_, _closure_, _funciones de orden superior_ y
       _composición_.
  - Familiarizarnos con un lenguaje funcional.
     - Despejando el misterio o las creencias que hay sobre _"programar sin variables"_,
       _"programar sin ciclos for, while, do-while"_ o _"programar sin efectos secundarios"_.

## Lo que no busco

  - Explicar _la teoría_ de programación funcional como si fuera una lista de conceptos sin uso
    práctico en la programación cotidiana.
  - Explicar _las entrañas_ de Clojure o el como están implementadas las _"ideas avanzadas"_.
  - Abordar las herramientas propias de Clojure para pruebas unitarias, análisis estático de
    código, formateo de código, despliegue de una aplicación, etc.
  - Confrontar las preferencias personales para programar: lenguajes, paradigmas, editores de
    texto, sintaxis, _tipado_, etc.

## Lo que te recomiendo

  - **_des_-aprender para aprender**
     - Algunas ideas en la programación funcional son contrarias a las ideas
       promovidas en la _programación imperativa/orientada a objetos_ (PI/OO).
       En el caso de Clojure podemos leer
       [Object Orientation is overrated](https://clojure.org/about/rationale#_object_orientation_is_overrated)
     - Nos será de gran ayuda dejar a un lado las _"buenas prácticas de programación"_ promovidas
       por la PI/OO.
  - **esencia contra implementación**
     - Es normal cuestionarse el como funcionan las cosas, sin embargo es más importante
       concentrarse en la esencia de las cosas para su uso o aprovechamiento.
  - **intuición contra formalidad**
     - Conocer conceptos _primitivos_ o _esenciales_ en cierto orden y con cierto grado de rigidez
       nos ayuda a comprender conceptos _complejos_ paulatinamente.
  - **lo importante contra lo urgente**
     - Es posible que busquemos un beneficio inmediato en aquello que usamos, debido a una necesidad
       o una presión que no controlamos del todo. Ante esto, es posible que no prestemos la
      debida atención a lo importante de lo que usamos, a aquellos que podría beneficiarnos en otras
      situaciones en un posible futuro.

# Sobre Clojure

Clojure es un _lenguaje de programación funcional_ encontrado en distintas plataformas o entornos
de ejecución, así como un lenguaje de programación que ha influenciado a otros:

- [Oficial: Java Virtual Machine](https://clojure.org/about/jvm_hosted)
- [GraalVM Native Image](https://github.com/clj-easy/graalvm-clojure)
- [ClojureScript: Javascript / NodeJS](https://clojure.org/about/clojurescript)
- [ClojureCLR: C# / .NET CLR](https://clojure.org/about/clojureclr)
- [Babashka: shell script](https://github.com/babashka/babashka)
- [jank: LLVM / C++](https://github.com/jank-lang/jank)
- [phel: PHP](https://github.com/phel-lang/phel-lang)
- [Carp: Haskell](https://github.com/carp-lang/Carp)
- [Ferret: C++11](https://ferret-lang.org)
- [hy: Python](https://github.com/hylang/hy)
- [clojerl: Erlang VM](https://github.com/clojerl/clojerl)
- [Fennel: Lua](https://github.com/bakpakin/Fennel)
- [Joker: Go](https://github.com/candid82/joker)
- [ClojureRS: Rust](https://github.com/clojure-rs/ClojureRS)

Cuenta con varias [historias de éxito](https://clojure.org/community/success_stories), siendo usado
por [compañías de distinto tamaño alrededor del mundo](https://clojure.org/community/companies),
incluyendo a empresas como _Apple_, _CircleCI_, _Heroku_, _Nubank_ y _Walmart_. Vale la pena
mencionar la existencia de [comunidades de usuarios](https://clojure.org/community/user_groups) en
distintos países.

## Observaciones

# Entorno de trabajo

## Java

## Leiningen

## VSCode & Calva

## Proyecto

# Créditos

# Copyright and License

Copyright (c) 2022 [Antonio Hernández Blas](https://nihilipster.dev)

Distributed under the [MIT license](LICENSE)
