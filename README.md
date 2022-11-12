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

El entorno de desarrollo está basado en el uso de Java, Leiningen y VSCode.

## Java

Se utilizará la
[JVM (Java Virtual Machine)](https://es.wikipedia.org/wiki/M%C3%A1quina_virtual_Java) como
anfitrión de Clojure, para lo cual se hace uso de la versión **17** del
[Java Development Kit (JDK)](https://es.wikipedia.org/wiki/Java_Development_Kit), ofrecido por el
proyecto [Eclipse Adoptium Temurin](https://adoptium.net):

    $ which java
    /usr/bin/java
    $ java -version
    openjdk version "17.0.5" 2022-10-18
    OpenJDK Runtime Environment Temurin-17.0.5+8 (build 17.0.5+8)
    OpenJDK 64-Bit Server VM Temurin-17.0.5+8 (build 17.0.5+8, mixed mode, sharing)
    $ which javac
    /usr/bin/javac
    $ javac -version
    javac 17.0.5

**Notas**:

- Es posible hacer uso de la versión **11** del JDK.
- El proyecto [SDKMAN!](https://sdkman.io/install) permite la instalación del JDK en los sistemas
  operativos principales (MS Windows, GNU/Linux y macOS):

      $ sdk install java 17.0.5-tem

## Leiningen

[Leiningen](https://leiningen.org) ayuda a la administración de proyectos en Clojure, permitiendo
su creación, el manejo de sus dependencias, su ejecutarlo, su empaquetado, así como ejecutar un
*REPL* como parte del mismo.

    $ which lein
    /usr/bin/lein
    $ lein version
    Leiningen 2.9.7 on Java 17.0.5 OpenJDK 64-Bit Server VM

**Notas**:

- Podemos seguir
  [las indicaciones dadas para su instalación](https://codeberg.org/leiningen/leiningen#installation)
  o bien instalarlo mediante SDKMAN!:

      $ sdk install leiningen

## VSCode

[Visual Studio Code](https://code.visualstudio.com) es un editor de texto gratuito, el cual
se puede descargar desde <https://code.visualstudio.com/download>.

### Calva

[Calva](https://marketplace.visualstudio.com/items?itemName=betterthantomorrow.calva) es un _plugin_
que otorga un _entorno de desarrollo_ a Visual Studio Code para programar en Clojure y _ClojureScript_.

La documentación de Calva se encuentra en <https://calva.readthedocs.io>.

# REPL

Las siguientes instrucciones nos permitirán por un lado verificar que nuestro entorno de trabajo se
encuentre correctamente configurado, una vez instalado los anteriores programas, y por otro lado
nos permitirá tener un primer contacto con Clojure.

## REPL con Leiningen

Para acceder a un REPL ejecuta el comando `lein repl` en un terminal o consola de tu sistema
operativo:

    $ lein repl
    nREPL server started on port 53812 on host 127.0.0.1 - nrepl://127.0.0.1:53812
    REPL-y 0.5.1, nREPL 0.8.3
    Clojure 1.10.3
    OpenJDK 64-Bit Server VM 17.0.5+8
        Docs: (doc function-name-here)
              (find-doc "part-of-name-here")
      Source: (source function-name-here)
     Javadoc: (javadoc java-object-or-class-here)
        Exit: Control+D or (exit) or (quit)
     Results: Stored in vars *1, *2, *3, an exception in *e
    
    user=>

Para salir del REPL evalua la expresión `(exit)` en el *prompt* (`user=>`) del REPL:

    user=> (exit)
    Bye for now!

## REPL en VSCode

Te será necesario crear un proyecto de Clojure mediante Leiningen y *cargar* dicho proyecto en
VSCode para acceder a un REPL.

Para crear un proyecto en Clojure ejecuta el comando `lein new <nombre del proyecto>`, por ejemplo:

    $  lein new proyecto-de-clojure
    Generating a project called proyecto-de-clojure based on the 'default' template.
    The default template is intended for library projects, not applications.
    To see other templates (app, plugin, etc), try `lein help new`.

En VSCode abre la carpeta `proyecto-de-clojure` recientemente creada.

Una vez *cargado* el proyecto de Clojure en VSCode da click sobre el botón **REPL**
(ubicado en la barra inferior de VSCode), selecciona la opción **Start your proyect with a REPL and
connect (a.k.a jack-in)** y posteriormente la opción *Leiningen*.

Como resultado podrás hacer uso del REPL mediante la pestaña *output.calva-repl*, evaluando
expresiones en el *prompt* (`clj:proyecto-de-clojure.core:>`) del REPL.

## Video

En el siguiente video podrás encontrar las mismas instrucciones expuestas en los anteriores puntos
para configurar a VSCode y Calva, así como los pasos para ejecutar un REPL en VSCode.

<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/6uUynWkMDGM"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
</iframe>

# Créditos

# Copyright and License

Copyright (c) 2022 [Antonio Hernández Blas](https://nihilipster.dev)

Distributed under the [MIT license](LICENSE)
