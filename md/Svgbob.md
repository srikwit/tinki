# Svgbob

Svgbob is a diagramming model
which uses a set of typing characters
to approximate the intended shape.

```bob
       .---.
      /-o-/--
   .-/ / /->
  ( *  \/
   '-.  \
      \ /
       '
```
It uses a [combination of characters](Svgbob/Specification.md)
which are readily available on your keyboards.

What can it do?

#### Basic shapes

```bob
    .- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -.
    !                                                    .            :
    !   +------+   .------.    .------.      /\        .' `.          :
    !   |      |   |      |   (        )    /  \     .'     `.   ^    :
    !   +------+   '------'    '------'    '----'     `.   .'   /   # :
    !     _______            ________               #   `.'    / ^ /  :
    !    /       \      /\   \       \     o---->   | ^       # / /   :
    !   /         \    /  \   )       )    <----#   | |  ^ :   / v    :
    !   \         /    \  /  /_______/              v |  ! :          :
    !    \_______/      \/             o.             o  ! V          :
    !                                    `.~~~~.                      :
    !                                           '.         O          :
    !    .-----------.       .   <.      .>  .    '.     ^  \         :
    !   (             )     (      )    (     )    :      \  \        :
    !    '-----+ ,---'       `>   '      `  <'     '.~~~~> \  v       :
    !          |/                                           *         :
    !          '                                       _        __    :
    !        __   .-.   .--.   .--.--.     .--.      .' '.    ,'  '.  :
    !   (_) (__) (   ) (    ) (  ( )  )   (    )    (     )  (      ) :
    !             '-'   `--'   `--'--'     `--'      `._.'    `.__.'  :
    !                                                                 !
    !      ___        ____         ____           _____               !
    !    ,'   `.    ,'    `.     .'    `.       ,'     `.             !
    !   /       \  /        \   /        \     /         \            !
    !   \       /  \        /  (          )   (           )           !
    !    `.___.'    `.____.'    \        /     \         /            !
    !                            `.____.'       `._____.'             !
    !        ______                                                   !
    !      ,'      `.                                                 !
    !     /          \    .-----. .----.                              !
    !    |            |    \   /   \    \                             !
    !    |            |     \ /     \    \                            !
    !     \          /       '       '----'                           !
    !      `.______.'                                                 !
    !                                                                 !
    `~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~'
```

#### Quick logo scribbles

```bob
        .---.                      _
       /-o-/--       .--.         |-|               .--.
    .-/ / /->       /--. \     .--)-|    .--.-.    //.-.\
   ( *  \/         / O  )|     |  |-|    |->| |   (+(-*-))
    '-.  \        /\ |-//      .  * |    '--'-'    \\'-'/
       \ /        \ '+'/        \__/                '--'
        '          '--'

       .----.               _
       |    |           ,--(_)
     __|____|__       _/ .-. \
    |  ______--|     (_)(   ) )
    `-/.::::.\-'       \ `-'_/
     `--------'         `--(_)

```
#### Box drawing

 Even unicode box drawing characters are supported

```bob
            ┌─┬┐  ╔═╦╗  ╓─╥╖  ╒═╤╕
            ├─┼┤  ╠═╬╣  ╟─╫╢  ╞═╪╡
            └─┴┘  ╚═╩╝  ╙─╨╜  ╘═╧╛
            ╭─┬╮
            ├─┼┤
            ╰─┴╯
```


 #### Grids

```bob


    .----.        .----.
   /      \      /      \            .-----+-----+-----.
  +        +----+        +----.      |     |     |     |          .-----+-----+-----+-----+
   \      /      \      /      \     |     |     |     |         /     /     /     /     /
    +----+        +----+        +    +-----+-----+-----+        +-----+-----+-----+-----+
   /      \      /      \      /     |     |     |     |       /     /     /     /     /
  +        +----+        +----+      |     |     |     |      +-----+-----+-----+-----+
   \      /      \      /      \     +-----+-----+-----+     /     /     /     /     /
    '----+        +----+        +    |     |     |     |    +-----+-----+-----+-----+
          \      /      \      /     |     |     |     |   /     /     /     /     /
           '----'        '----'      '-----+-----+-----'  '-----+-----+-----+-----+





       ___     ___      .---+---+---+---+---.     .---+---+---+---.  .---.   .---.
   ___/   \___/   \     |   |   |   |   |   |    / \ / \ / \ / \ /   |   +---+   |
  /   \___/   \___/     +---+---+---+---+---+   +---+---+---+---+    +---+   +---+
  \___/   \___/   \     |   |   |   |   |   |    \ / \ / \ / \ / \   |   +---+   |
  /   \___/   \___/     +---+---+---+---+---+     +---+---+---+---+  +---+   +---+
  \___/   \___/   \     |   |   |   |   |   |    / \ / \ / \ / \ /   |   +---+   |
      \___/   \___/     '---+---+---+---+---'   '---+---+---+---'    '---'   '---'

```

#### Graphics Diagram

```bob
                                                                             .
    0       3                          P *              Eye /         ^     /
     *-------*      +y                    \                +)          \   /  Reflection
  1 /|    2 /|       ^                     \                \           \ v
   *-------* |       |                v0    \     ^ v3           --------*--------
   | |4    | |7      | ◄╮               *----\---/-*
   | *-----|-*     ⤹ +-----> +x        /      v /   \          .-.<--------        o
   |/      |/       / ⤴               /        o     \        ( / ) Refraction    / \
   *-------*       v                 /                \        '-'               /   \
  5       6      +z              v1 *------------------* v2    |                o-----o
                                                               v

```

#### Sequence Diagrams

```bob

                                   .--->  F
          A       B      C  D     /
          *-------*-----*---*----*----->  E
                   \            ^ \
                    v          /   '--->  G
                     B --> C -'


                          ,-.
                          `-'
                          /|\
         ,---.             |
         |Bob|            / \
         `-+-'           Alice
           |    hello      |
           |-------------->|
           |               |
           |  Is it ok?    |
           |<- - - - - - - |
         ,-+-.           Alice
         |Bob|            ,-.
         `---'            `-'
                          /|\
                           |
                          / \


              .─.
             ( 0 )
              `-'
            /     \
           /       \
          V         V
         .─.         .─.
        ( 1 )       ( 4 )
         `-'         `-' .
       /   \         |  \ `.
      /     \        |   \  `.
     V       V       |    \   `.
    .─.      .─.     V     V    V
   ( 2 )    ( 3 )    .─.   .─.   .─.
    `─'      `─'    ( 5 ) ( 6 ) ( 7 )
                     `─'   `─'   `─'

```

#### Railroad diagrams

```bob
               ┌------┐   .-.  ┌---┐
        o--╮---| elem |--( ; )-| n |--╭--o
           |   └------┘   `-'  └---┘  |
           | ╭------>------╮          |
           | |    ┌---┐    |          |
           ╰-╯-╭--| x |--╮-╰----------╯
           |   |  └---┘  |            |
           |   |   .-.   |            |
           |   `--( , )--'            ^
           |       `-'                |
           |  ╭-------->---------╮    |
           |  |   ┌---┐   .-.    |    |
           ╰--╰-╭-| x |--( , )-╮-╯----╯
                | └---┘   `-'  |
                `-------<------'
                                       .------------>---------------.
           ┌-------------┐  .-.   .-.  |  ┌------┐  .-.   ┌-----┐   |    .-.   ┌------┐
      O____| struct_name |_( : )_( | )_◞__| name |_( : )__| tpe |___◟___( | )__| body |______O
        ◝  └-------------┘  `-'   `-'   ◜ └------┘  `-'   └-----┘  ◝     `-'   └------┘  ◜
        |                               |                    .-.   |                     |
        |                               `------------<------( , )--'                     |
        |                                                    `-'                         |
        `--------------------------------------------------------------------------------'

```

#### Statistical charts

```bob

    E +-------------------------*--+     E |                         o
    D |-------------------*--*--|--*     D |                   o  o  |  o
    C |-------------*--*  |  |  |  |     C |             o  o  |  |  |  |
    B |-------*--*  |  |  |  |  |  |     B |       o  o  |  |  |  |  |  |
    A +-*--*--+--+--+--+--+--+--+--+     A +-o--o--|--|--|--|--|--|--|--|
        5 10 15 20 25 30 35 40 45 50         5 10 15 20 25 30 35 40 45 50



  85.67 ┤                                       ╭╮
  78.20 ┤                                       ││                  ╭╮
  70.73 ┤                                       ││  ╭╮ ╭╮ ╭╮   ╭╮  ╭╯╰─╮
  63.27 ┤                        ╭╮         ╭─╮ ││ ╭╯╰╮│╰─╯╰╮╭╮│╰──╯   │╭
  55.80 ┤   ╭╮                 ╭╮││╭╮ ╭╮╭╮  │ ╰─╯╰─╯  ││    ││││       ╰╯
  48.33 ┤   │╰╮      ╭──╮      │││││╰╮│╰╯│  │         ╰╯    ╰╯╰╯
  40.87 ┤╭╮ │ ╰╮╭╮  ╭╯  ╰─╮╭╮╭─╯╰╯╰╯ ╰╯  ╰──╯
  33.40 ┤││ │  ╰╯╰╮╭╯     ││╰╯
  25.93 ┤││╭╯     ╰╯      ╰╯
  18.47 ┼╯││
  11.00 ┤ ╰╯
        └───────────┴───────────┴───────────┴───────────┴───────────┴────
      2011        2012        2013        2014        2015        2016


```




#### Flow charts

```bob
                      .--.            .---.  .---. .---.  .---.    .---.  .---.
                      |  |   OS API   '---'  '---' '---'  '---'    '---'  '---'
                      v  |              |      |     |      |        |      |
             .-. .-. .-. |              v      v     |      v        |      v
         .-->'-' '-' '-' |            .------------. | .-----------. |  .-----.
         |     \  |  /   |            | Filesystem | | | Scheduler | |  | MMU |
         |      v . v    |            '------------' | '-----------' |  '-----'
         |_______/ \_____|                   |       |      |        |
                 \ /                         v       |      |        v
                  |     ____              .----.     |      |    .---------.
                  '--> /___/              | IO |<----'      |    | Network |
                                          '----'            |    '---------'
                                             |              |         |
                                             v              v         v
                                      .---------------------------------------.
                                      |                  HAL                  |
                                      '---------------------------------------'


             .---.  .---. .---.  .---.    .---.  .---.
    OS API   '---'  '---' '---'  '---'    '---'  '---'
               |      |     |      |        |      |
               v      v     |      v        |      v
             .------------. | .-----------. |  .-----.
             |  文件系统  | | |   调度器  | |  | MMU |
             '------------' | '-----------' |  '-----'
                    |       |      |        |
                    v       |      |        v
                 .----.     |      |    .---------.
                 | IO |<----'      |    |   网络  |
                 '----'            |    '---------'
                    |              |         |
                    v              v         v
             .---------------------------------------.
             |              硬件抽象层               |
             '---------------------------------------'
```

#### Block diagrams

```bob

      vncviewer         .-,(  ),-.
       __  _         .-(          )-.           gateway           vncserver
      [__]|=|  ---->(    internet    )-------> __________ ------> ____   __
     /⠶⠶ /|_|        '-(          ).-'        [_...__...°]       |    | |==|
                         '-.( ).-'                               |____| |  |
                                                                 /⠶⠶⠶ / |__|


                              Valveless --------.
                            Pulsejet engine    /
                                              V
                               _________.------------------+
                    .---------'                           /  -------->
                   /  .-------._________                  \   thrust-->
                  (  (      _________   `-----------o------+  -------->
                   \  `----'         '----'         |
                    `------._  __^___.----.         |
                             ||  |                  |
                   fuel  __^ ||  | ^__spark         |GND
                  intake     ||  |    plug          |
                             ||  |                  |
                             ||  |                  |
                         ____||  `------------.     |
                        / .---'               |     |
                        | |                   |     |              +-+-+-+-+-+
                    .---| |---.   __          |     |              |-+-+-+-+-|
                 ___|  +-+-+--|--o  `---------*-----|--------------O-+-+-+-+-|
       .-------> ___  ||||||| |  power        |     *--------------O-+-+-+-+-|
        \           | ||||||| |  switch       |     |              |-+-+-+-+-|
          Water     `-+-+-+-+-'            +--o-----o--+           +-+-+-+-+-+
          intake       HHO                 |           |
                      Generator            |  +     -  |            Solar panel
                                           +-----------+
                                              Battery

               =======
                =====  symbolic antenna
                 ===
                  =
                  |
                  |          micro henry
                  |          coil w/tuning lug
                  |    .----.
                  |   (.-') |
                  |   (.-') |
                  |   (.-') |      pico farad cap
                  |   (.-'  |    ___  (trimmable)
                  |   |     |   |___|
        PC   ->  .----'-----'---'---'
        Board    `-------------------
                 ground plane (foil)

```


#### Mindmaps

```bob

                                            .-->  Alpha
                                           /
                                          .---->  Initial Release
          Planning *-------.             /         \
                            \           /           '---> Patch 1
      Initial research       \         /             \
                *             \       /               '-->  Patch 2
                 \             \     .---------> Beta
                  \             \   /
                   \             o o                      _______
                    \          .---. *--.___             /       \
                     '------> (     )       '------O->  . Release .
                               `---' o                   \_______/
                               o  o o \
                              /    \ \ \
                          .--'      \ \ \
                         /           \ \ '----+->  Push backs
                        .             \ \      \
                       /|              \ \      '----> Setbacks
                      / .               \ \
                     V /|                \ '-----> Reception
                Team  / .                 \
                     v /|                  \
             Worklaod / .                   '-->> Career change
                     V /
                 PTO  /
                     V
                 Bug

```

#### Circuit diagrams

  It can do complex stuff such as circuit diagrams

```bob

       +10-15V           ___0,047R
      *---------o-----o-|___|-o--o---------o----o-------.
    + |         |     |       |  |         |    |       |
    -===-      _|_    |       | .+.        |    |       |
    -===-      .-.    |       | | | 2k2    |    |       |
    -===-    470| +   |       | | |        |    |      _|_
    - |       uF|     '--.    | '+'       .+.   |      \ / LED
      +---------o        |6   |7 |8    1k | |   |      -+-
             ___|___   .-+----+--+--.     | |   |       |
              -═══-    |            |     '+'   |       |
                -      |            |1     |  |/  BC    |
               GND     |            +------o--+   547   |
                       |            |      |  |`>       |
                       |            |     ,+.   |       |
               .-------+            | 220R| |   o----||-+  IRF9Z34
               |       |            |     | |   |    |+->
               |       |  MC34063   |     `+'   |    ||-+
               |       |            |      |    |       |  BYV29     -12V6
               |       |            |      '----'       o--|<-o----o--X OUT
 6000 micro  - | +     |            |2                  |     |    |
 Farad, 40V ___|_____  |            |--o                C|    |    |
 Capacitor  ~ ~ ~ ~ ~  |            | GND         30uH  C|    |   --- 470
               |       |            |3      1nF         C|    |   ###  uF
               |       |            |-------||--.       |     |    | +
               |       '-----+----+-'           |      GND    |   GND
               |            5|   4|             |             |
               |             |    '-------------o-------------o
               |             |                           ___  |
               `-------------*------/\/\/------------o--|___|-'
                                     2k              |       1k0
                                                    .+.
                                                    | | 5k6 + 3k3
                                                    | | in Serie
                                                    '+'
                                                     |
                                                    GND

```

### Advantages

 - Plain text format
    - Ultimately portable, backward compatible and future proof.
 - Degrades gracefully
    - Even when not using a graphical renderer, it would still looks good
    as text based diagrams.
 - Easiest to use.
    - Anyone knows how to edit text.

### Goal
- Make the rendered shape closely resembles to that of the textual representation.

### NON-goals
- To be able to make graphs and diagrams with less effort.
- To replace standard diagramming tools.


#### Links
- [Svgbob specification](Svgbob/Specification.md)
- [Circle specification](Svgbob/Circles.md)
- [Design architecture](Svgbob/Architecture.md)
- [Design implementation](Svgbob/Design-Implementation.md)
- [Code Respository](https://github.com/ivanceras/svgbob)
- [Svgbob live editor](https://ivanceras.github.io/svgbob-editor) - an online editor which lets you easily create svgbob drawing
