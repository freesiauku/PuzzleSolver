# Puzzles Solvers & OR tutorials

[![EN](https://img.shields.io/badge/Lang-EN-blue.svg)](https://github.com/SmilingWayne/PuzzleSolver/blob/main/README.md)
[![CN](https://img.shields.io/badge/中文-CN-red.svg)](https://github.com/SmilingWayne/PuzzleSolver/blob/main/README.CN.md)

This repo provides useful, problem-tailored solvers for some interesting **logic puzzles**. The main tool I used in the repo is Google Operations Research software [ORtools](https://developers.google.cn/optimization?hl=zh-cn), especially its CS-SAT solver. Commercial solver [Gurobi](https://www.gurobi.com) (Licence required, of course) is also used for specific puzzle (Like [Slitherlink](./Puzzles/SlitherLink.ipynb)). 

Most other solvers of those problems are based on logical methods, instead, this repo provides solvers based on mathematical Programming (Integer Programming(**IP**), Constraint Programming(**CP**) etc..). Just In case, I must say I always admire those who quickly come up with logic-based solutions for those problems, and this repo is **NOT** aimed at replacing logic method with Computer solvers. This repo is just for fun.

Besides, **this repo also contains some dataset ( 2000+ instances for now) of specific puzzles**. Details can be found in catalog. More dataset would be added in the future.

Lastly, this repo also contains some self-learning materials for Operations Research (**OR**).

✅ Python Environment: Python 3.10.12, 

✅ Gurobi Optimizer Version: 10.0.3.

✅ ortools Optimizer Version: 9.7.2996


## Catalog

-------

### Sudoku and variants puzzles 

1. [Ortools for diversified Sudoku-like Puzzles](./Puzzles.ipynb): 🥰 The very beginning of my repo. In this note, most of the sudokus (and variants) are well-designed so <u>you can easily add or integrate different constraints types and solve comprehensive Sudoku grid</u>, such as **"Killer sudoku with Thermo Constraints"** or **"Anti-Knight Diagnoal Sudoku"**. A very good example can be found [Here](https://cn.gridpuzzle.com/sudoku-puzzles?page=3). 


### Other logic Puzzles

1. [**Solvers for Logic Puzzles using CS-SAT or MILP**](./Puzzles/). More INTERESTING and brain-burning logic puzzles. Including path-finding, digit-filling and flag-placing puzzles. The puzzles that have been solved:

![](./assets/figures/Headers.png)
![](./assets/figures/Headers2.png)


> Table of Sudoku and its variants, with dataset. 👇

|  ID   |  Sudoku & variants   |  In Chinese  | Done & Tested |                              Note                              | Dataset size | # of dataset | With Sol? |
| :---: | :------------------: | :----------: | :-----------: | :------------------------------------------------------------: | :----------: | :----------: | :-------: |
|   1   |   Standard Sudoku    |   标准数独   |       ✅       |         [Rules](https://en.gridpuzzle.com/rule/sudoku)         |     9x9      |      -       |     -     |
|   2   |    Killer Sudoku     |   杀手数独   |       ✅       |     [Rules](https://en.gridpuzzle.com/rule/killer-sudoku)      |     9x9      |     155      |     ✅     |
|   3   |    Jigsaw Sudoku     |   锯齿数独   |       ✅       |     [Rules](https://en.gridpuzzle.com/rule/jigsaw-sudoku)      |     9x9      |     128      |     ✅     |
|   4   |  Consecutive Sudoku  |   连续数独   |       ✅       |   [Rules](https://en.gridpuzzle.com/rule/consecutive-sudoku)   |     9x9      |      -       |     -     |
|   5   |   Sandwich Sudoku    |  三明治数独  |       ✅       |    [Rules](https://en.gridpuzzle.com/rule/sandwich-sudoku)     |     9x9      |      -       |     -     |
|   6   |  Thermometer Sudoku  |  温度计数独  |       ✅       |     [Rules](https://www.sudoku-variants.com/thermo-sudoku)     |     9x9      |      -       |     -     |
|   7   | Petite-Killer Sudoku |  小杀手数独  |       ✅       | [Rules](https://sudoku-puzzles.net/little-killer-sudoku-hard/) |     9x9      |      -       |     -     |
|   8   |  Anti-Knight Sudoku  |   无马数独   |       ✅       |   [Rules](https://en.gridpuzzle.com/rule/anti-knight-sudoku)   |     9x9      |      -       |     -     |
|   9   |   Anti-King Sudoku   |   无缘数独   |       ✅       |    [Rules](https://en.gridpuzzle.com/rule/anti-king-sudoku)    |     9x9      |      -       |     -     |
|  10   | Greater-Than Sudoku  |  不等式数独  |       ✅       | [Rules](https://sudoku-puzzles.net/greater-than-sudoku-hard/)  |     9x9      |      -       |     -     |
|  11   |   Diagonal Sudoku    |  对角线数独  |       ✅       |       [Rules](https://en.gridpuzzle.com/diagonal-sudoku)       |     9x9      |      -       |     -     |
|  12   |        Vudoku        |   V宫数独    |       ✅       |           [Rules](https://en.gridpuzzle.com/vsudoku)           |     9x9      |      -       |     -     |
|  13   |     Arrow Sudoku     |   箭头数独   |       ✅       |         [Rules](https://www.sudoku-variants.com/arrow)         |     9x9      |      -       |     -     |
|  14   |      XV Sudoku       |    XV数独    |       ✅       |       [Rules](https://en.gridpuzzle.com/rule/vx-sudoku)        |     9x9      |      -       |     -     |
|  15   |    Window Sudoku     |   窗口数独   |       ✅       |        [Rules](https://en.gridpuzzle.com/rule/windoku)         |     9x9      |      -       |     -     |
|  16   |    Kropki Sudoku     |  黑白点数独  |       ✅       |        [Rules](https://en.gridpuzzle.com/kropki-sudoku)        |     9x9      |      -       |     -     |
|  17   |   Even-Odd Sudoku    |   奇偶数独   |       ✅       |    [Rules](https://en.gridpuzzle.com/rule/even-odd-sudoku)     |     9x9      |     129      |     ✅     |
|  18   |    Samurai Sudoku    |   武士数独   |       🐌       |                               -                                |    21x21     |     272      |     ✅     |
|  19   |    Shogun Sudoku     |   将军数独   |       🐌       |                               -                                |    21x45     |      90      |     ✅     |
|  20   |     Sumo Sudoku      |   Sumo数独   |       🐌       |                               -                                |    33x33     |     110      |     ✅     |
|  21   |     Sohei Sudoku     |  Sohei数独   |       🐌       |                               -                                |    21x21     |     120      |     ✅     |
|  22   |   Clueless Sudoku2   | 无提示数独2  |       🐌       |                               -                                |    27x27     |      40      |     ✅     |
|  23   |   Butterfly Sudoku   |   蝴蝶数独   |       🐌       |                               -                                |    12x12     |      77      |     ✅     |
|  24   |   Windmill Sudoku    |   风车数独   |       🐌       |                               -                                |    21x21     |     150      |     ✅     |
|  25   |   Gattai-8 Sudoku    | Gattai-8数独 |       🐌       |                               -                                |    21x33     |     120      |     ✅     |
|  26   |   Clueless Sudoku1   | 无提示数独1  |       🐌       |                               -                                |    27x27     |      29      |     ✅     |



> Table of Other Puzzles 👇.

|  ID   |                       Name of Other Puzzles                       | Chinese Translation | Solved? |                                      Note                                      |                  Dataset                  |
| :---: | :---------------------------------------------------------------: | :-----------------: | :-----: | :----------------------------------------------------------------------------: | :---------------------------------------: |
|   1   |             [Alphadoku](./Puzzles/Alphabetoku.ipynb)              |   25 by 25 字母独   |    ✅    |                                       -                                        |                     -                     |
|   2   |       [Akari](./Puzzles/Akari.ipynb) <br> (aka: light UP!)        |        照明         |    ✅    |                    [Rules](https://www.puzzle-light-up.com)                    |                 💪 Working                 |
|   3   |  [Cryptarithmetic](./Puzzles/Cryptarithmetic.ipynb) <br> Puzzles  |      破译密码       |    ✅    |                                       -                                        |                     -                     |
|   4   |               [Norinori](./Puzzles/NoriNori.ipynb)                |        海苔         |    ✅    |                    [Rules](https://www.puzzle-norinori.com)                    |                 💪 Working                 |
|   5   |             [Number Link](./Puzzles/NumberLink.ipynb)             |        数链         |    🐌    |                                       -                                        |                 💪 Working                 |
|   6   |            [Minesweeper](./Puzzles/Minesweeper.ipynb)             |      静态扫雷       |    ✅    |                                       -                                        |                     -                     |
|   7   |   [Simple Loop](./Puzzles/SimpleLoop.ipynb) <br> (aka: Loopy~)    |      简单回路       |    ✅    |                               🚀 Gurobi required                                |                     -                     |
|   8   |            [Siltherlink](./Puzzles/SlitherLink.ipynb)             |         环          |    ✅    | 🚀 Gurobi required, [rules](https://www.janko.at/Raetsel/Slitherlink/index.htm) | [dataset](./assets/data/slitherlinkdata/) |
|   9   |                 [Mosaic](./Puzzles/Mosaic.ipynb)                  |       马赛克        |    ✅    |          [Rules](https://www.puzzle-minesweeper.com/mosaic-5x5-easy/)          |     [dataset](./assets/data/Mosaic/)      |
|  10   |                   [Tent](./Puzzles/Tent.ipynb)                    |        帐篷         |    ✅    |                     [Rules](https://www.puzzle-tents.com)                      |                 💪 Working                 |
|  11   |               [Nonogram](./Puzzles/Nonogram.ipynb)                |        数织         |    ✅    |          No use of ortools, [rules](https://www.puzzle-nonograms.com)          |                 💪 Working                 |
|  12   |                [Aquaium](./Puzzles/Aquarium.ipynb)                |        水箱         |    ✅    |                                       -                                        |                     -                     |
|  13   |               [Kakurasu](./Puzzles/Kakurasu.ipynb)                |       方阵和        |    ✅    |            [Rules](https://www.janko.at/Raetsel/Kakurasu/index.htm)            |                 💪 Working                 |
|  14   |             [Starbattle](./Puzzles/Starbattle.ipynb)              |        星战         |    ✅    |                                       -                                        |                     -                     |
|  15   |                               LITS                                |        LITS         |    ❌    |                                       -                                        |                     -                     |
|  16   |              [Pentomino](./Puzzles/Pentomino.ipynb)               |      五联骨牌       |    ✅    |                  [Rules](https://isomerdesign.com/Pentomino/)                  |                 💪 Working                 |
|  17   |                 [Suguru](./Puzzles/Suguru.ipynb)                  |          🤔️          |    ✅    |             [Rules](https://puzzlegenius.org/suguru-from-scratch/)             |                 💪 Working                 |
|  18   |                [Shikaku](./Puzzles/Shikaku.ipynb)                 |        直角         |    ❌    |                [Rules](https://www.puzzle-shikaku.com/?size=5)                 |                     -                     |
|  19   |                 [Kakuro](./Puzzles/Kakuro.ipynb)                  |       交叉和        |    ✅    |             [Rules](https://www.janko.at/Raetsel/Kakuro/index.htm)             |                     -                     |
|  20   |                [Binario](./Puzzles/Binario.ipynb)                 |       二进制        |    ✅    |                    [Rules](https://www.puzzle-binairo.com)                     |                 💪 Working                 |
|  21   |  [Five Cells](./Puzzles/FiveCells.ipynb) <br> (aka: Faibuseruzu)  |       五空格        |    ✅    |            [Rules](https://www.cross-plus-a.com/html/cros7fzu.htm)             |                     -                     |
|  22   | [Fobidoshi](./Puzzles/Fobidoshi.ipynb) <br> (aka: Forbidden Four) |      禁止四连       |    ✅    |                 [Rules](https://www.cross-plus-a.com/help.htm)                 |                     -                     |
|  23   |                 [Hitori](./Puzzles/Hitori.ipynb)                  |      请勿打扰       |    ✅    |   🚀 Gurobi required, [rules](https://www.janko.at/Raetsel/Hitori/index.htm)    |     [dataset](./assets/data/hitori/)      |
|  24   |               [Monotone](./Puzzles/Monotone.ipynb)                |       单调性        |    ✅    |                               🚀 Gurobi required                                |                     -                     |
|  25   |                  [Creek](./Puzzles/Creek.ipynb)                   |        小溪         |    ✅    |    🚀 Gurobi required, [rules](https://www.janko.at/Raetsel/Creek/index.htm)    |                 💪 Working                 |
|  26   |     [Patchwork](./Puzzles/Patchwork.ipynb) <br> (aka: Tatami)     |       榻榻米        |    ✅    |                 [Rules](https://www.cross-plus-a.com/help.htm)                 |                     -                     |
|  27   |                [Kalkulu](./Puzzles/Kalkulu.ipynb)                 |      解谜游戏       |    ✅    |            [Rules](https://www.janko.at/Raetsel/Kalkulu/index.htm)             |                     -                     |
|  28   |               [Heyawake](./Puzzles/Heyawake.ipynb)                |      Heyawake       |    ✅    |            [Rules](https://www.janko.at/Raetsel/Heyawake/index.htm)            |                 💪 Working                 |
|  29   |                  [Gappy](./Puzzles/Gappy.ipynb)                   |        盖比!        |    ✅    |             [Rules](https://www.janko.at/Raetsel/Gappy/index.htm)              |      [dataset](./assets/data/Gappy/)      |
|  30   |              [GrandTour](./Puzzles/GrandTour.ipynb)               |        旅途         |    ✅    |    🚀 Gurobi required, [Rules](https://www.janko.at/Raetsel/Gappy/index.htm)    |    [dataset](./assets/data/GrandTour/)    |
|  31   |         [Honeycomb](./Puzzles/Honeycomb.ipynb) <br> 1 & 2         |        蜂巢         |    ✅    |     🚀 Gurobi required, [Rules](https://matmod.ch/lpl/HTML/honeycomb.html)      |                     -                     |
|  32   |              [Maze-A-pix](./Puzzles/MazeAPix.ipynb)               |      迷宫绘画       |    ✅    |   [Rules](https://www.conceptispuzzles.com/index.aspx?uri=puzzle/maze-a-pix)   |                     -                     |

----

### Dataset of some puzzles

- Many puzzle sources found online are in PDF format, which **makes it difficult to use them directly for automated solving**. For that reason, this repository also offers easy-to-use web crawlers that extract puzzle data in a structured format, rather than as images or PDF data. See [Utils](./Utils/). **Currently, we support structured data and corresponding final solutions for over 2,000 puzzles across 20+ different puzzle types**. A detailed list of the available datasets is provided below. Please note that Sudoku datasets are already covered in a previous section and are omitted here.

- Additionally, **for puzzles where bulk datasets are not yet available, at least one test case is provided to validate the correctness of the solving algorithm**. Contributions of more datasets are welcome and encouraged.

|  ID   |                  Puzzle name                  |                                   Size of puzzle                                    |                       # of puzzle                       | With Sol? |
| :---: | :-------------------------------------------: | :---------------------------------------------------------------------------------: | :-----------------------------------------------------: | :-------: |
|   1   | [SlitherLink](./assets/data/slitherlinkdata/) | 10x18 <br> 14x24 <br> 20x36 <br> 20x30 <br> 16x19 <br> 30x25 <br> 60x60 <br> Others | 220 <br> 91 <br> 58 <br>33 <br> 28 <br>9 <br> 1 <br> 44 |     ✅     |
|   2   |        [Mosaic](./assets/data/Mosaic/)        |                            25x25 <br> 15x15 <br> Others                             |                   38 <br> 40 <br> 26                    |     ✅     |
|   3   |         [Gappy](./assets/data/Gappy/)         |                                        12x12                                        |                           60                            |     ✅     |
|   4   |        [Hitori](./assets/data/hitori/)        |                                  17x17  <br> 10x10                                  |                      153  <br> 172                      |     ✅     |
|   5   |     [GrandTour](./assets/data/GrandTour/)     |                                        11x11                                        |                           126                           |     ✅     |
|   6   |         [Akari](./assets/data/Akari/)         |             14x24 <br> 23 x 33 <br> 17 x 17  <br> 100x100   <br> Others             |            72 <br> 17 <br> 18 <br> 1 <br> 21            |     ✅     |




-----

### Some OR materials 

This section contains several materials when learning(and coding) Operations Research. Mostly IP and CP, with some classical Combinatorial Optimization Problems. More appendix, like mathematical models, can be found in [Notes](https://smilingwayne.github.io/me/OROpt/) (Written in Mandarin) on my personal website.

1. [Ortools for Linear Programming](./ORMaterials/SimpleLP.ipynb) : Tutorials.
2. [Ortools for Mixed Integer Programming](./ORMaterials/IntegerOpt.ipynb): Tutorials.
3. [Ortools for Constraint Programming](./ORMaterials/ConstraintOpt.ipynb): Tutorials.
4. [Ortools for Knapsack Problem](./ORMaterials/KnapsackPro.ipynb): Tutorials.
5. [Ortools for VRP](./ORMaterials/VRP): Variants and ortools codes( of official website for self-learning).
6. [Ortools & Gurobi for TSP](./ORMaterials/TSP.ipynb): Two main methods for TSP. 
7. [Column Generation Method: Large-Scale Linear Programming and Cutting Stock Problems](./ORMaterials/Techniques/ColGen/CSP.ipynb): Team Meeting report.
8. Branch & Price for Parallel Machine Scheduling: 🐌...
9. Some basic / classic [Operations Research Modeling](./modeling/) :


----

## Reference

- [ORtools Official](https://developers.google.cn/optimization?hl=zh-cn)
- [Hakank's ORtools tutorials](http://www.hakank.org/google_or_tools/)
- Puzzle data: [Raetsel's Janko](https://www.janko.at/Raetsel/index.htm), [Puzzle](https://www.puzzle-loop.com)
