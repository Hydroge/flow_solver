# flow_solver（English）

**Original repository: <https://github.com/mzucker/flow_solver>, and the code here is edited & improved by Hydroge.**

Fast automated solver for Flow Free in a single C or Python file. 

Full writeup of C version at <https://mzucker.github.io/2016/08/28/flow-solver.html>.

Python writeup at <https://mzucker.github.io/2016/09/02/eating-sat-flavored-crow.html>.

## Building the C version

No dependencies to install, just do this:

    cd /path/to/flow_solver
    mkdir build
    cd build
    cmake .. -DCMAKE_BUILD_TYPE=Release
    make

Or you can compile this .c file directly with DEV-C++.

Visual Studio is NOT recommended, for it reports too many problems.

## Using the C version:

From the `build` directory or the root directory of this ".exe" file, try:

    ./flow_solver ../puzzles/jumbo_14x14_01.txt
    
## Using the Python version:

Make sure you have [pycosat](https://github.com/ContinuumIO/pycosat) installed. If not, try:

    pip install pycosat
    
Then, from the project root directory, try:

    ./pyflowsolver.py puzzles/jumbo_14x14_01.txt

## Puzzle file format

**WARNING: SOME CHANGES HAS BEEN MADE HERE, WITCH HAS MAKE THIS EDITION DIFFERENT FROM THE ORIGINAL VERSION.**

Plain-ASCII file, one line per row of puzzle. Use the following
characters to specify color:

| Letter | Color        |
|--------|--------------|
| A      | red          |
| C      | blue         |
| D      | yellow       |
| B      | green        |
| E      | orange       |
| F      | cyan         |
| I      | magenta      |
| H      | maroon       |
| P      | purple       |
| K      | gray         |
| J      | white        |
| L      | bright green |
| M      | tan          |
| N      | dark blue    |
| O      | dark cyan    |
| P      | pink         |

Any non-alphabetical, non-newline character becomes a blank space.
Puzzle size is set by the number of characters before the first
newline.

**Note that after the puzzle, you need to begin another blank line!**

# 连接同色点-计算器（中文版

**原仓库链接: <https://github.com/mzucker/flow_solver>, 此处的版本由Hydroge加以改进。**

用单个c文件或Python源文件即可实现快速且自动化的连接同色点计算功能。

C版本的编写思路：<https://mzucker.github.io/2016/08/28/flow-solver.html>.

Python版本的编写思路：<https://mzucker.github.io/2016/09/02/eating-sat-flavored-crow.html>.

## C语言编译

不需要安装额外的东西，只需要按照下面的操作即可。

    cd /path/to/flow_solver
    mkdir build
    cd build
    cmake .. -DCMAKE_BUILD_TYPE=Release
    make

或者您可以直接使用Dev-C++对该.c文件进行编译。

**不推荐**使用Visual Studio，因为其会报出大量的错误。

## 使用C语言这版本

在命令提示符中的build链接（或者.exe所在的链接），让软件读取一个符合格式的.txt文件（详情见releases）。例如：

    ./flow_solver ../puzzles/jumbo_14x14_01.txt
    
## 使用Python版本:

在保证您已经安装[pycosat](https://github.com/ContinuumIO/pycosat)的情况下使用本程序。若未安装，可以通过以下指令进行安装：

    pip install pycosat
    
定位到.py文件所在的根目录，让软件读取一个符合格式的.txt文件（详情见releases）。例如:

    ./pyflowsolver.py puzzles/jumbo_14x14_01.txt

## 谜题文件格式

**WARNING: SOME CHANGES HAS BEEN MADE HERE, WITCH HAS MAKE THIS EDITION DIFFERENT FROM THE ORIGINAL VERSION.**

**警告：此处作出了一些修改，使得该版本的计算器与原网站的计算器不同**

普通的ASCII文件，文件的一行代表谜题的一行。使用以下字母来表示颜色：

| Letter | Color        |
|--------|--------------|
| A      | red 红色          |
| C      | blue 蓝色        |
| D      | yellow 黄色      |
| B      | green 绿色       |
| E      | orange 橙色      |
| F      | cyan 青色        |
| I      | magenta 洋红     |
| H      | maroon 褐红色      |
| P      | purple 紫色      |
| K      | gray 灰色        |
| J      | white 白色       |
| L      | bright green 亮绿色|
| M      | tan 棕褐色         |
| N      | dark blue 暗蓝色   |
| O      | dark cyan 暗青色   |
| P      | pink 粉色        |

Any non-alphabetical, non-newline character becomes a blank space.
Puzzle size is set by the number of characters before the first
newline.

任何非字母、非换行符的字符都会变成空白。

拼图大小由第一个换行符前的字符数设置。

**注意，在谜题之后，还需另起一个空行！**

