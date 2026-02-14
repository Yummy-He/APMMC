由AI从文档中提取的代码块，在这里可以方便地复制：

# 0. 写在前面
## 0.1 关于本笔记
暂无本小节代码块。

## 0.2 章节结构
### 代码 0.2.1
```
这是第0节第1小节第1个代码块。
```

### 代码 0.2.2
```
这是第0节第1小节第2个代码块。
```

## 0.3 字体
### 代码 0.3.1
```
一二三四五六七八九十百千万
AbCdEfGhIjKlMnOpQrStUvWxYz
```

## 0.4 内容
暂无本小节代码块。


# 1. Linux入门
## 1.1 Linux简介
暂无本小节代码块。

## 1.2 Linux的特点
暂无本小节代码块。

## 1.3 Linux的安装
### 代码 1.3.1
```
user@host:~$ sudo passwd root
```

## 1.4 Linux的文件结构与目录相关操作
### 代码 1.4.1
```
user1@host:~$ pwd
/home/user1
```

### 代码 1.4.2
```
user1@host:~$ cd /home/user1
```

### 代码 1.4.3
```
user1@host:~$ cd ~
```

### 代码 1.4.4
```
user1@host:~$ mkdir test
```

### 代码 1.4.5
```
user1@host:~$ mkdir ~/test/test1
user1@host:~$ mkdir ~/test/test1/test2 ~/test/test1/test3
```

### 代码 1.4.6
```
user1@host:~$ mkdir -p ~/test/test1/test2
```

### 代码 1.4.7
```
user1@host:~$ rmdir ~/test/test1/test3
```

### 代码 1.4.8
```
user1@host:~$ cd ~/test/test1
```

### 代码 1.4.9
```
user1@host:~/test/test1$ touch 1.txt
```

### 代码 1.4.10
```
user1@host:~/test/test1$ touch 1.txt 2.txt
```

### 代码 1.4.11
```
user1@host:~/test/test1$ ls
1.txt  2.txt  test2
```

### 代码 1.4.12
```
user1@host:~/test/test1$ cd ./test2
```

### 代码 1.4.13
```
user1@host:~/test/test1/test2$ cd ..
```

### 代码 1.4.14
```
user1@host:~/test/test1$ cp 1.txt test2/
```

### 代码 1.4.15
```
user1@host:~/test/test1$ cp 1.txt test2/3.txt
```

### 代码 1.4.16
```
user1@host:~/test/test1$ mv test2/1.txt test2/.4.txt
```

### 代码 1.4.17
```
cp [选项] 源文件1 源文件2 ... 目标目录
mv [选项] 源文件1 源文件2 ... 目标目录
```

### 代码 1.4.18
```
ls [选项] [目录]
```

### 代码 1.4.19
```
user1@host:~/test/test1$ ls -a ~/test
.  ..  1.txt  2.txt  test2

user1@host:~/test/test1$ ls -l
总计 4
-rw-rw-r-- 1 user1 user1    0  7月  1 12:48 1.txt
-rw-rw-r-- 1 user1 user1    0  7月  1 12:48 2.txt
drwxrwxr-x 2 user1 user1 4096  7月  1 12:47 test2

user1@host:~/test/test1$ ls -a
.  ..  1.txt  2.txt  test2

user1@host:~/test/test1$ ls -R
.:
1.txt  2.txt  test2

./test2:
1.txt

user1@host:~/test/test1$ ls -aR
.:
.  ..  1.txt  2.txt  test2

./test2:
.  ..  1.txt  .4.txt

user1@host:~/test/test1$ ls -alR
.:
总计 12
drwxrwxr-x 3 user1 user1 4096  7月  1 12:48 .
drwxrwxr-x 3 user1 user1 4096  7月  1 12:47 ..
-rw-rw-r-- 1 user1 user1    0  7月  1 12:48 1.txt
-rw-rw-r-- 1 user1 user1    0  7月  1 12:48 2.txt
drwxrwxr-x 2 user1 user1 4096  7月  1 12:53 test2

./test2:
总计 8
drwxrwxr-x 2 user1 user1 4096  7月  1 12:53 .
drwxrwxr-x 3 user1 user1 4096  7月  1 12:48 ..
-rw-rw-r-- 1 user1 user1    0  7月  1 12:53 1.txt
-rw-rw-r-- 1 user1 user1    0  7月  1 12:53 .4.txt
```

### 代码 1.4.20
```
user1@host:~/test/test1$ rm 1.txt
```

### 代码 1.4.21
```
user1@host:~/test/test1$ cd ..
user1@host:~/test$ rm -r test1
```

### 代码 1.4.22
```
mkdir [-p] 目录1 目录2 ...
rmdir 目录1 目录2 ...
touch 文件1 文件2 ...
```

### 代码 1.4.23
```
cp [-r,-i] 源文件1 源文件2 ... 目标目录
mv [-i] 源文件1 源文件2 ... 目标目录
```

### 代码 1.4.24
```
ls [-l,-a,-R] [目录]
```

### 代码 1.4.25
```
rm [-i,-r,-f] 文件1 文件2 ... 目录1 目录2 ...
```

## 1.5 文件操作命令
### 代码 1.5.1
```
user1@host:~$ ls > list.txt
```

### 代码 1.5.2
```
user1@host:~$ ls >> list.txt
```

### 代码 1.5.3
```
user1@host:~$ ls non_existing_file 2> error.log
```

### 代码 1.5.4
```
user1@host:~$ echo "Hello, World!"
Hello, World!
user1@host:~$ echo "Hello, World!" > test/hello.txt
```

### 代码 1.5.5
```
user1@host:~$ echo "I'm Linux." >> test/hello.txt
user1@host:~$ echo "I'm also Ubuntu." >> test/hello.txt
```

### 代码 1.5.6
```
Hello, World!
I'm Linux.
I'm also Ubuntu.
```

### 代码 1.5.7
```
user1@host:~$ ls -l | grep .txt
```

### 代码 1.5.8
```
user1@host:~$ rm *.txt
```

### 代码 1.5.9
```
user1@host:~$ cat test/hello.txt
Hello, World!
I'm Linux.
I'm also Ubuntu.
user1@host:~$ cat -n test/hello.txt
1  Hello, World!
2  I'm Linux.
3  I'm also Ubuntu.
```

### 代码 1.5.10
```
user1@host:~$ shuf -r -n 300 -i 1-100 > test/numbers.txt
```

### 代码 1.5.11
```
user1@host:~$ less test/numbers.txt
```

### 代码 1.5.12
```
user1@host:~$ head test/numbers.txt
```

### 代码 1.5.13
```
user1@host:~$ head -n 20 test/numbers.txt
```

### 代码 1.5.14
```
user1@host:~$ head -n 20 test/numbers.txt | tail -n 10
user1@host:~$ head -n 20 test/numbers.txt | tail -n 5 > test/numbers16-20.txt
```

### 代码 1.5.15
```
user1@host:~$ find ./test -name "*.txt"
./test/numbers.txt
./test/hello.txt
```

### 代码 1.5.16
```
user1@host:~$ find ./test -user user1
./test/numbers.txt
./test/hello.txt
```

### 代码 1.5.17
```
user1@host:~$ which ls
/bin/ls
user1@host:~$ which find
/usr/bin/find
```

### 代码 1.5.18
```
user1@host:~$ whereis ls
ls: /bin/ls /usr/share/man/man1/ls.1.gz
user1@host:~$ whereis find
find: /usr/bin/find /usr/share/man/man1/find.1.gz /usr/share/info/find.info.gz
```

## 1.6 用户与文件权限管理
### 代码 1.6.1
```
user1@host:~$ sudo usermod -aG sudo user2
```

### 代码 1.6.2
```
user1@host:~$ sudo useradd user2
user1@host:~$ sudo passwd user2
```

### 代码 1.6.3
```
user1@host:~$ sudo chown user2 test/numbers.txt
user1@host:~$ sudo chown -R user2 test/
```

### 代码 1.6.4
```
user1@host:~$ sudo chgrp group1 test/numbers.txt
user1@host:~$ sudo chgrp -R group1 test/
```

### 代码 1.6.5
```
user1@host:~$ sudo chmod 755 test/numbers.txt
user1@host:~$ sudo chmod u=rwx,g=rx,o=rx test/numbers.txt
```

### 代码 1.6.6
```
user1@host:~$ sudo chmod u+x test/numbers.txt
user1@host:~$ sudo chmod g-w test/numbers.txt
```

## 1.7 为系统安装软件
### 代码 1.7.1
```
user1@host:~$ sudo apt-get update
```

### 代码 1.7.2
```
user1@host:~$ sudo apt-get install fortune
```

### 代码 1.7.3
```
user1@host:~$ fortune
```

### 代码 1.7.4
```
user1@host:~$ sudo apt-get install sl
```

### 代码 1.7.5
```
user1@host:~$ sl
```

### 代码 1.7.6
```
user1@host:~$ sudo apt-get remove fortune
```

### 代码 1.7.7
```
user1@host:~$ sudo apt-get install gfortran
```

### 代码 1.7.8
```
user1@host:~$ gfortran --version
GNU Fortran (Ubuntu 13.3.0-6ubuntu2~24.04) 13.3.0
Copyright (C) 2023 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

## 1.8 文本处理工具
### 代码 1.8.1
```
grep [选项] PATTERN [FILE...]
```

### 代码 1.8.2
```
user1@host:~$ grep -n 5 test/numbers.txt
```

### 代码 1.8.3
```
user1@host:~$ grep -nw 15 test/numbers.txt
```

### 代码 1.8.4
```
user1@host:~$ grep -G '^[0-9]\{3\}$' test/numbers.txt
```

### 代码 1.8.5
```
user1@host:~$ sudo apt-get install rs
user1@host:~$ seq 1 100 > test/numbers-2.txt
user1@host:~$ shuf -r -n 300 -i 60-100 >> test/numbers-2.txt
user1@host:~$ rs 4 100 < test/numbers-2.txt | rs -T > test/grades.txt
```

### 代码 1.8.6
```
user1@host:~$ awk '{print $1, ($2 + $3 + $4) / 3}' test/grades.txt
```

### 代码 1.8.7
```
user1@host:~$ awk '{print $1, $2, $3, $4, ($2 + $3 + $4) / 3}' test/grades.txt > test/grades-averages.txt
```

### 代码 1.8.8
```
sed [选项] '命令' [文件...]
```

### 代码 1.8.9
```
user1@host:~$ sed 's/60/70/g' test/grades.txt
```

### 代码 1.8.10
```
user1@host:~$ sed -i 's/60/70/g' test/grades.txt
```

## 1.9 Vim文本编辑器
### 代码 1.9.1
```
user1@host:~$ vimtutor zh
```

### 代码 1.9.2
```
user1@host:~$ vim test/grades.txt
```

### 代码 1.9.3
```
:wq
```

## 1.10 与window宿主机共享文件
暂无本小节代码块。


# 2. Fortran 语言简介
## 2.1 编程语言与Fortran的发展
暂无本小节代码块。

## 2.2 Fortran 与打孔卡片
### 代码 2.2.1
```
0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ,.:;'"-+=!@#$%^&*()_/<>
```

### 代码 2.2.2
```
C THE FIRST FORTRAN PROGRAM
      WRITE(6,10)
   10 FORMAT(1X, 'HELLO, WORLD.')
      END
```

### 代码 2.2.3
```
 HELLO, WORLD.
```


# 3. Fortran基础
## 3.1 Fortran语言的编译
### 代码 3.1.1
```
user1@host:~$ sudo apt-get install gfortran
```

### 代码 3.1.2
```
user1@host:~$ mkdir learn
user1@host:~$ cd learn
user1@host:~/learn$ vim hello.f
```

### 代码 3.1.3
```
C THE FIRST FORTRAN PROGRAM
      WRITE(6,10)
   10 FORMAT(1X, 'HELLO, WORLD.')
      END
```

### 代码 3.1.4
```
user1@host:~$ gfortran -c file.f -o customfilename.o
user1@host:~$ gfortran -o executablefilename customfilename.o
```

### 代码 3.1.5
```
user1@host:~/learn$ gfortran -c hello.f
user1@host:~/learn$ gfortran -o hello hello.o
user1@host:~/learn$ ls
hello  hello.f  hello.o
```

### 代码 3.1.6
```
user1@host:~/learn$ ./hello
 HELLO, WORLD.
```

### 代码 3.1.7
```
user1@host:~/learn$ sudo chmod 755 hello
```

### 代码 3.1.8
```
user1@host:~/learn$ gfortran -o hello hello.f
user1@host:~/learn$ ./hello
 HELLO, WORLD.
```

### 代码 3.1.9
```
user1@host:~/learn$ gfortran -c binom.f ifact.f
user1@host:~/learn$ ls
binom.f  binom.o  ifact.f  ifact.o
user1@host:~/learn$ gfortran -o binom binom.o ifact.o
user1@host:~/learn$ ls
binom  binom.f  binom.o  ifact.f  ifact.o
```

## 3.2 Fortran变量类型声明与转化
### 代码 3.2.1
```
      INTEGER :: I
      REAL :: X
      DOUBLE PRECISION :: Y
```

### 代码 3.2.2
```
      M = INT(A)
      N = IFIX(B)
      I = IDINT(C)
```

### 代码 3.2.3
```
      X = REAL(I)
      Y = FLOAT(J)
      Z = DBLE(K)
```

## 3.3 Fortran程序的输入与输出
### 代码 3.3.1
```
      READ, 变量
      READ(单位, 格式) 变量1 变量2 ...
```

### 代码 3.3.2
```
      WRITE(单位, 格式) 变量1 变量2 ...
```

### 代码 3.3.3
```
      PRINT(格式) 变量1 变量2 ...
```

## 3.4 格式化输出
### 代码 3.4.1
```
      WRITE(6, '(A, I5, F10.2, E10.2)') '结果是：', I, X
```

### 代码 3.4.2
```
      WRITE(6, 100) I, X
  100 FORMAT('结果是：', I5, F10.2, E10.2)
```

### 代码 3.4.3
```
      M=12345
      N=123
      K=123456
      WRITE(6, '(I5)') M
      WRITE(6, '(I5)') N
      WRITE(6, '(I5)') K
      END
```

### 代码 3.4.4
```
12345
  123
*****
```

### 代码 3.4.5
```
      K=1234567890
      X=123.456
      WRITE(6, '(I10)') K
      WRITE(6, '(F10.2)') X
      END
```

### 代码 3.4.6
```
1234567890
    123.46
```

### 代码 3.4.7
```
      K=1234567890
      Y=-123.456
      Z=123.456
      WRITE(6, '(I10)') K
      WRITE(6, '(E10.3)') Y      
      WRITE(6, '(E10.3)') Z
      END
```

### 代码 3.4.8
```
1234567890
-0.123E+03
 0.123E+03
```

## 3.5 数学语句
### 代码 3.5.1
```
      A = ABS(X)       ! 绝对值
      B = SQRT(Y)      ! 平方根
      C = EXP(Z)       ! 指数函数
      D = LOG(W)       ! 自然对数
      E = LOG10(V)     ! 常用对数
      F = SIN(T)       ! 正弦函数
      G = COS(U)       ! 余弦函数
      M = MAX(A, B)    ! 最大值
      N = MIN(C, D)    ! 最小值
      O = MOD(P, Q)    ! 取模
```

### 代码 3.5.2
```
      I = 5
      X = 3.14
      Y = 2.718281828459045
```

### 代码 3.5.3
```
      Z = X + Y
      A = B - C
      D = E * F
      G = H / I
      J = K ** L
```

### 代码 3.5.4
```
      Z = (EXP(X+Y) + SIN(X) + S**T) / (ABS(X) + SQRT(Y) - LOG10(W))
```

### 代码 3.5.5
```
      P = EXP(X+Y) + SIN(X) + S**T
      Q = ABS(X) + SQRT(Y) - LOG10(W)
      Z = P / Q
```

## 3.6 数组与下标变量
### 代码 3.6.1
```
C 一维数组（50个元素，存储学生学号）
      INTEGER ID(50)  ! 合并类型声明与维数声明
C 二维数组（25行4列，存储25名学生4门考试成绩）
      REAL SCORE(25,4)  ! 行=学生序号，列=考试科目
      
C 数组元素引用赋值示例
      ID(1) = 2024001  ! 第一个学生学号
      SCORE(2,3) = 92.5  ! 第二个学生第三门考试成绩
      WRITE(6, '(I8, F10.1)') ID(1), SCORE(2,3)
      END
```

### 代码 3.6.2
```
C 独立DIMENSION语句声明
      DIMENSION ARR1(100), ARR2(3,5), ARR3(2,4,3)
      INTEGER ARR1, ARR3  ! 声明数组类型
      REAL ARR2           ! 二维数组存储实数
      
C 合并类型与维数声明（推荐）
      INTEGER :: STUDENT(50)  ! 50个学生的整数类型数据
      REAL :: MATRIX(10,10)   ! 10×10的实数矩阵
      
C 错误声明示例（禁止）
C     INTEGER N=5
C     DIMENSION ERR(3, N)  ! 维度不能用变量N
C     DIMENSION ERR2(0,4)  ! 下标不能为0
      END
```

### 代码 3.6.3
```
      DIMENSION A(10), B(3,4), C(2,2,2)
      INTEGER K=3, M=2
      
C 合法下标引用
      A(5) = 10.0        ! 常量下标
      A(K+2) = 20.0      ! 表达式下标（K+2=5）
      B(2, M*2) = 30.0   ! 二维数组，M*2=4（列下标）
      C(1,2,2) = 40.0    ! 三维数组，第2页、第2列、第1行
      
C 非法下标引用（禁止使用）
C     A(0) = 5.0        ! 零下标
C     A(-1) = 8.0       ! 负下标
C     B(3,5) = 15.0     ! 列下标超界（声明为4列）
C     C(2, M(1)) = 25.0 ! 数组作为下标
      
      WRITE(6, '(F8.1, F8.1, F8.1, F8.1)') A(5), A(5), B(2,4), C(1,2,2)
      END
```

### 代码 3.6.4
```
C 数组I/O示例：25名学生4门考试成绩的读写
      DIMENSION SCORE(25,4), AVE(25)
      REAL SUM
      
C 隐式DO循环输入（按行读入每个学生的4门成绩）
      READ(5, '(4F10.1)') ((SCORE(I,J), J=1,4), I=1,25)
      
C 数组名直接输出（按存储顺序输出所有成绩，列优先）
      WRITE(6, '(1X, 4F10.1)') SCORE
      
C DO循环计算并输出每个学生的平均分
      DO 100 I=1,25
          SUM=0.0
          DO 200 J=1,4
              SUM=SUM+SCORE(I,J)
200       CONTINUE
          AVE(I)=SUM/4.0
100   CONTINUE
C 嵌套隐式DO循环输出学号、成绩、平均分
      WRITE(6, '(1X, I3, 4F10.1, F10.2)') ((I, SCORE(I,J), J=1,4, AVE(I)), I=1,25)
      
      END
```

### 代码 3.6.5
```
C 三维数组（2页×3列×4行）的读写
      DIMENSION C(4,3,2)  ! 行=4，列=3，页=2
      
C 嵌套隐式DO循环输入（页→列→行顺序）
      READ(5, '(6F8.1)') (((C(I,J,K), I=1,4), J=1,3), K=1,2)
      
C 嵌套隐式DO循环输出（按页分行打印）
      DO 100 K=1,2
          WRITE(6, '(1X, A, I1)') 'PAGE ', K
          WRITE(6, '(1X, 3F8.1)') ((C(I,J,K), J=1,3), I=1,4)
100   CONTINUE
      
      END
```


# 4. Fortran程序结构
## 4.1 Fortran程序构成和子程序
### 代码 4.1.1
```
      PROGRAM HelloWorld
      INTEGER :: I
      REAL :: X, Y
      
      WRITE(6, '(A)') 'Hello, World!'
      
      I = 5
      X = 3.14
      Y = 2.718281828459045
      
      WRITE(6, '(I5, F10.2, E10.3)') I, X, Y
      
      END PROGRAM HelloWorld
```

### 代码 4.1.2
```
C FUNCTION SUBPROGRAM: COMPUTE K FACTORIAL
      FUNCTION IFACT(K)
      INTEGER IFACT, K, J
      IFACT = 1
      IF(K.EQ.0) RETURN
      DO 10 J = 1, K
          IFACT = IFACT * J
10    CONTINUE
      RETURN
      END
```

### 代码 4.1.3
```
C MAIN PROGRAM: CALCULATE BINOMIAL COEFFICIENT
      INTEGER UP, DOWN, IBINQ, N, I
      READ(5, *) N, I
      UP = IFACT(N)
      DOWN = IFACT(N-I) * IFACT(I)
      IBINQ = UP / DOWN
      WRITE(6, 20) N, I, IBINQ
20    FORMAT(6X, 'N=', I5, 5X, 'I=', I5, 5X, 'BINOMIAL COEFF=', I8)
      STOP
      END
```

### 代码 4.1.4
```
user1@host:~/learn$ gfortran -c binom.f ifact.f
user1@host:~/learn$ gfortran -o binom binom.o ifact.o
user1@host:~/learn$ ./binom
8,3
      N=    8     I=    3     BINOMIAL COEFF=      56
```

### 代码 4.1.5
```
C SUBROUTINE TO INTCHG TWO NUMBERS
      SUBROUTINE INTCHG(A, B)
      REAL :: A, B, TEMP
      TEMP = A
      A = B
      B = TEMP
      RETURN
      END
```

### 代码 4.1.6
```
C MAIN PROGRAM: CALL INTCHG TO SWAP TWO NUMBERS
      REAL A, B
      A = 5.5
      B = 10.2
      WRITE(6, 10) A, B
10    FORMAT(1X, 'BEFORE SWAP: A=', F5.1, 2X, 'B=', F5.1)
      CALL INTCHG(A, B)
      WRITE(6, 20) A, B
20    FORMAT(1X, 'AFTER SWAP: A=', F5.1, 2X, 'B=', F5.1)
      STOP
      END
```

### 代码 4.1.7
```
user1@host:~/learn$ gfortran -c testswap.f swap.f
user1@host:~/learn$ gfortran -o testswap testswap.o swap.o
user1@host:~/learn$ ./testswap
BEFORE SWAP: A= 5.5  B=10.2
AFTER SWAP: A=10.2  B= 5.5
```

### 代码 4.1.8
```
C MAIN PROGRAM WITH ARITHMETIC STATEMENT FUNCTION
      REAL G, X, VALUE
      INTEGER J
C DEFINE STATEMENT FUNCTION
      G(X) = X*X - 5.0*X + 2.0
C CALCULATE AND PRINT VALUES
      DO 100 J = 1, 20
          X = FLOAT(J)
          VALUE = G(X)
          WRITE(6, 10) J, VALUE
10        FORMAT(1X, 'X=', I3, 2X, 'G(X)=', F8.2)
100   CONTINUE
      STOP
      END
```

### 代码 4.1.9
```
user1@host:~/learn$ ./statfunc
X=  1  G(X)=  -2.00
X=  2  G(X)=  -4.00
X=  3  G(X)=  -4.00
X=  4  G(X)=  -2.00
· · ·
```

## 4.2 IF语句
### 代码 4.2.1
```
      IF(X.GT.0) WRITE(6,*)X,Y
```

### 代码 4.2.2
```
      IF(X.GT.0) THEN
          Y = X**2
          WRITE(6,*)Y
      ENDIF
```

### 代码 4.2.3
```
      IF(X.GT.0) THEN
          IF(Y.LT.0) THEN
              Z = X + Y
          ELSE
              Z = X - Y
          ENDIF
      ENDIF
```

### 代码 4.2.4
```
      IF(X) 10, 20, 30
10    WRITE(6,*) 'X < 0'
20    WRITE(6,*) 'X = 0'
30    WRITE(6,*) 'X > 0'
```

### 代码 4.2.5
```
      IF(ABS(X - TARGET).LT..00001) THEN
          ...
      ENDIF
```

## 4.3 GOTO语句
### 代码 4.3.1
```
      INTEGER I
      I = 1
10    CONTINUE
      IF(I.GT.100) GOTO 20
      I = I + 1
      GOTO 10
20    CONTINUE
      END
```

### 代码 4.3.2
```
      INTEGER I
      I = 1
10    IF(I.GT.100) GOTO 20
      I = I + 1
      GOTO 10
20    END
```

### 代码 4.3.3
```
      GOTO (10, 20, 30) N
10    WRITE(6,*) 'N = 1'
20    WRITE(6,*) 'N = 2'
30    WRITE(6,*) 'N = 3'
      END
```

## 4.4 DO循环语句
### 代码 4.4.1
```
      DO LABEL VAR = START, END, STEP
          ! 循环体
LABEL CONTINUE
```

### 代码 4.4.2
```
      INTEGER I, SUM
      SUM = 0
      DO 10 I = 1, 10
          SUM = SUM + I
10    CONTINUE
      WRITE(6,*) '1到10的整数和为：', SUM
      END
```

### 代码 4.4.3
```
      INTEGER I, SUM
      SUM = 0
      DO I = 1, 10
          SUM = SUM + I
      END DO
      WRITE(6,*) '1到10的整数和为：', SUM
      END
```

### 代码 4.4.4
```
      INTEGER I, J, SUM
      INTEGER, DIMENSION(3, 3) :: A
      ! 初始化数组A
      A = RESHAPE([1, 2, 3, 4, 5, 6, 7, 8, 9], [3, 3])
      SUM = 0
      DO 10 I = 1, 3
          DO 20 J = 1, 3
              SUM = SUM + A(I, J)
20        CONTINUE
10    CONTINUE
      WRITE(6,*) '二维数组元素和为：', SUM
      END
```

## 4.5 程序框图
暂无本小节代码块。


# 5. 程序实例
## 5.1 循环与基本计算实例
### 代码 5.1.1
```
user1@host:~$ mkdir examples
user1@host:~$ cd examples
user1@host:~/examples$ vim sum1.f
```

### 代码 5.1.2
```
      READ(5,*) A,B,N
      SUM=0.0
      DO I=0,N-1
          SUM=SUM+1.0/(A+I*B)
      END DO
      WRITE(6,*) SUM
      END
```

### 代码 5.1.3
```
user1@host:~/examples$ gfortran -o sum1 sum1.f
user1@host:~/examples$ ./sum1
1 2 10
   2.13325596
```

### 代码 5.1.4
```
      READ(5,*) N
      PROD=1.0
      DO I=1,N
          PROD=PROD*(2.0*I-1.0)/(I*I)
      END DO
      WRITE(6,*) PROD
      END
```

### 代码 5.1.5
```
user1@host:~/examples$ gfortran -o prod1 prod1.f
user1@host:~/examples$ ./prod1
10
   4.97205074E-05
```

## 5.2 数值计算与条件判断实例
### 代码 5.2.1
```
      READ(5,*) S, EPS
      XN=S/2.0
      DO
          XN1=0.5*(XN+S/XN)
          IF (ABS(XN1-XN) .LT. EPS) THEN
              EXIT
          END IF
          XN=XN1
      END DO
      WRITE(6,*) XN1
      END
```

### 代码 5.2.2
```
      READ(5,*) A,B,C
      D=B*B-4.0*A*C
      IF (D .LT. 0.0) THEN
          WRITE(6,*) 'No real roots'
      ELSE
          R1=(-B+SQRT(D))/(2.0*A)
          R2=(-B-SQRT(D))/(2.0*A)
          WRITE(6,*) R1,R2
      END IF
      END
```

## 5.3 数据处理与数组实例
### 代码 5.3.1
```
      SUM=0.0
      SUMSQ=0.0
      ICOUNT=0
      XMAX=-1.0E30
      XMIN=1.0E30
      DO
          READ(5,*) X
          IF (X .EQ. 0.0) EXIT
          SUM=SUM+X
          SUMSQ=SUMSQ+X*X
          ICOUNT=ICOUNT+1
          IF (X .GT. XMAX) XMAX=X
          IF (X .LT. XMIN) XMIN=X
      END DO
      IF (ICOUNT .EQ. 0) THEN
          WRITE(6,*) 'No data entered'
      ELSE
          XMEAN=SUM/ICOUNT
          STDDEV=SQRT((SUMSQ-ICOUNT*XMEAN*XMEAN)/(ICOUNT-1))
          WRITE(6,10) XMAX, XMIN, XMEAN, STDDEV
   10     FORMAT('Max=',F10.4,' Min=',F10.4,
     &        ' Mean=',F10.4,' StdDev=',F10.4)
      END IF
      END
```

### 代码 5.3.2
```
user1@host:~/examples$ gfortran -o stats1 stats1.f
user1@host:~/examples$ ./stats1
12
13
14
15
15
15
16
17
18
0
Max=   18.0000 Min=   12.0000 Mean=   15.0000 StdDev=    1.8708
```

### 代码 5.3.3
```
      DIMENSION X(100)
      ICOUNT=0
      DO
          READ(5,*) X(ICOUNT+1)
          IF (X(ICOUNT+1) .EQ. 0.0) EXIT
          ICOUNT=ICOUNT+1
          IF (ICOUNT .GE. MAXN) THEN
              WRITE(6,*) 'Array full'
              EXIT
          END IF
      END DO
      IF (ICOUNT .EQ. 0) THEN
          WRITE(6,*) 'No data entered'
      ELSE
          XMAX=X(1)
          XMIN=X(1)
          SUM=0.0
          SUMSQ=0.0
          DO I=1,ICOUNT
              SUM=SUM+X(I)
              SUMSQ=SUMSQ+X(I)*X(I)
              IF (X(I) .GT. XMAX) XMAX=X(I)
              IF (X(I) .LT. XMIN) XMIN=X(I)
          END DO
          XMEAN=SUM/ICOUNT
          STDDEV=SQRT((SUMSQ-ICOUNT*XMEAN*XMEAN)/(ICOUNT-1))
          WRITE(6,10) XMAX, XMIN, XMEAN, STDDEV
   10     FORMAT('Max=',F10.4,' Min=',F10.4,
     &        ' Mean=',F10.4,' StdDev=',F10.4)
      END IF
      END
```

### 代码 5.3.4
```
      DIMENSION A(100)
      READ(5,*) N
      IF (N .GT. 100) THEN
        WRITE(6,*) 'Error: N too large'
        STOP
      ENDIF
      
      DO 10 I = 1, N
        READ(5,*) A(I)
   10 CONTINUE
      
      WRITE(6,*) 'Original array:'
      DO 20 I = 1, N
        WRITE(6,*) A(I)
   20 CONTINUE
      
      DO 30 I = 1, N-1
        DO 40 J = 1, N-I
          IF (A(J) .GT. A(J+1)) THEN
            TEMP = A(J)
            A(J) = A(J+1)
            A(J+1) = TEMP
          ENDIF
   40   CONTINUE
   30 CONTINUE
      
      WRITE(6,*) 'Sorted array:'
      DO 50 I = 1, N
        WRITE(6,*) A(I)
   50 CONTINUE
      END
```

### 代码 5.3.5
```
      INTEGER NF(100)
      READ(5,*) N
      IF (N .GT. 100) THEN
        WRITE(6,*) 'Error: N too large'
        STOP
      ENDIF

      NF(1) = 1
      NF(2) = 1
      DO 10 I = 3, N
        NF(I) = NF(I-1) + NF(I-2)
   10 CONTINUE
      
      WRITE(6,*) 'Fibonacci sequence:'
      DO 20 I = 1, N
        WRITE(6,*) NF(I)
   20 CONTINUE
      END
```

## 5.4 多维数组与矩阵运算实例
### 代码 5.4.1
```
user1@host:~$ sudo apt-get install rs
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 5 5 > matrix1.txt
```

### 代码 5.4.2
```
      PROGRAM DETERMINANT
C     ARRAY SIZE: MAXIMUM 100 X 100 MATRIX

      DIMENSION A(100,100), B(10000)
      LOGICAL NOSING
      CHARACTER LINE*1000
C
C     READ ALL NUMBERS FROM INPUT BY PROCESSING EACH LINE
      K = 0
      NLINE = 0
   10 READ(5,'(A)',END=20) LINE
C     PROCESS NON-EMPTY LINES
      IF (LINE .NE. ' ') THEN
        NLINE = NLINE + 1
        LENLINE = LEN(LINE)
C       PARSE NUMBERS FROM THE LINE
        IPOS = 1
   30   CONTINUE
C       FIND NEXT NON-BLANK CHARACTER
        DO WHILE (IPOS .LE. LENLINE .AND. LINE(IPOS:IPOS) .EQ. ' ')
          IPOS = IPOS + 1
        ENDDO
        IF (IPOS .GT. LENLINE) GOTO 40
C       FIND END OF CURRENT NUMBER
        J = IPOS
        DO WHILE (J .LE. LENLINE .AND. LINE(J:J) .NE. ' ')
          J = J + 1
        ENDDO
C       CONVERT SUBSTRING TO NUMBER
        IF (J .GT. IPOS) THEN
          READ(LINE(IPOS:J-1),*) B(K+1)
          K = K + 1
          IPOS = J
          GOTO 30
        ENDIF
   40   CONTINUE
      ENDIF
      GOTO 10
   20 CONTINUE
C
C     CHECK IF TOTAL COUNT IS PERFECT SQUARE
      N = NINT(SQRT(REAL(K)))
      IF (N*N .NE. K) THEN
        WRITE(6,*) 'ERROR: NUMBER OF ELEMENTS IS NOT PERFECT SQUARE'
        STOP
      ENDIF
C
C     FILL 2D MATRIX A FROM 1D ARRAY B (ROW-MAJOR ORDER)
      DO 50 I = 1, N
        DO 60 J = 1, N
          A(I,J) = B((I-1)*N + J)
   60   CONTINUE
   50 CONTINUE
C
      WRITE(6,*)'MATRIX:'
      DO K=1,N
      WRITE(6,'(100F10.2)') (A(I,K),I=1,N)
      END DO
      
C     CALCULATE DETERMINANT USING GAUSSIAN ELIMINATION
      DET = 1.0
      NOSING = .TRUE.
C
      DO 70 K = 1, N-1
C       FIND PIVOT ELEMENT (MAXIMUM IN COLUMN)
        PIV = ABS(A(K,K))
        IPIV = K
        DO 80 I = K+1, N
          IF (ABS(A(I,K)) .GT. PIV) THEN
            PIV = ABS(A(I,K))
            IPIV = I
          ENDIF
   80   CONTINUE
C
C       CHECK FOR SINGULAR MATRIX
        IF (PIV .EQ. 0.0) THEN
          NOSING = .FALSE.
          GOTO 90
        ENDIF
C
C       SWAP ROWS IF NECESSARY
        IF (IPIV .NE. K) THEN
          DET = -DET
          DO 100 J = 1, N
            TEMP = A(K,J)
            A(K,J) = A(IPIV,J)
            A(IPIV,J) = TEMP
  100     CONTINUE
        ENDIF
C
C       ELIMINATION PROCESS
        DO 110 I = K+1, N
          FACTOR = A(I,K)/A(K,K)
          DO 120 J = K+1, N
            A(I,J) = A(I,J) - FACTOR*A(K,J)
  120     CONTINUE
  110   CONTINUE
        DET = DET * A(K,K)
   70 CONTINUE
      DET = DET * A(N,N)
C
   90 CONTINUE
C
C     OUTPUT RESULT
      IF (NOSING) THEN
        WRITE(6, '(A, F10.2)') 'DETERMINANT = ', DET
      ELSE
        WRITE(6,*) 'SINGULAR MATRIX, DETERMINANT = 0'
      ENDIF
C
      STOP
      END
```

### 代码 5.4.3
```
user1@host:~/examples$ gfortran -o determinant determinant.f
user1@host:~/examples$ ./determinant < matrix1.txt
 MATRIX:
      7.00      9.00      5.00      9.00     10.00
      5.00      7.00      5.00      8.00      9.00
     10.00      7.00      7.00      7.00      9.00
     10.00      8.00      9.00      6.00     10.00
      7.00      7.00     10.00      6.00      9.00
DETERMINANT =     314.00
```

### 代码 5.4.4
```
      PROGRAM MATMUL
      IMPLICIT REAL*8 (A-H,O-Z)
      IMPLICIT INTEGER*4 (I-N)
C     DECLARE POINTERS FOR DYNAMIC ARRAYS
      REAL*8, POINTER :: A(:,:), B(:,:), C(:,:)
      
C     READ MATRIX DIMENSIONS
      READ(5,*) M, K, N
      
C     ALLOCATE MEMORY FOR MATRICES
      ALLOCATE(A(M,K), B(K,N), C(M,N))
      
C     READ MATRIX A (M x K)
      DO 10 I = 1, M
        READ(5,*) (A(I,J), J = 1, K)
10    CONTINUE
      
C     READ MATRIX B (K x N)
      DO 20 I = 1, K
        READ(5,*) (B(I,J), J = 1, N)
20    CONTINUE
      
C     PERFORM MATRIX MULTIPLICATION C = A * B
      DO 30 I = 1, M
        DO 40 J = 1, N
          C(I,J) = 0.0D0
          DO 50 L = 1, K
            C(I,J) = C(I,J) + A(I,L) * B(L,J)
50        CONTINUE
40      CONTINUE
30    CONTINUE
      
C     WRITE RESULT MATRIX C (M x N)
      WRITE(6,*) 'RESULT MATRIX C:'
      DO 60 I = 1, M
        WRITE(6,'(1000F16.4)') (C(I,J), J = 1, N)
60    CONTINUE
      
C     DEALLOCATE MEMORY
      DEALLOCATE(A)
      DEALLOCATE(B)
      DEALLOCATE(C)
      
      STOP
      END
```

### 代码 5.4.5
```
user1@host:~$ echo "2 3 2" >matrix2.txt
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 2 3 >> matrix2.txt
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 3 2 >> matrix2.txt
```

### 代码 5.4.6
```
user1@host:~/examples$ gfortran -o matmult matmult.f
user1@host:~/examples$ ./matmult < matrix2.txt
 RESULT MATRIX C:
        131.0000        133.0000
        135.0000        128.0000
```

## 5.5 化学中的应用实例
### 代码 5.5.1
```
user1@host:~/examples$ gfortran -o Mcal Mcal.f -fdefault-real-8
```

### 代码 5.5.2
```
user1@host:~/examples$ ./Mcal
 Target molecular weight: 
135.0684
 Minimal degree of unsaturation (e.g., 4.0): 
5
 Starting Genetic Algorithm optimization...
New GA best: FIT=    1.123200 SOL=   15.   13.    1.    1.    0.
New GA best: FIT=   33.439090 SOL=    6.    7.    1.    3.    0.
New GA best: FIT=   34.985004 SOL=    2.    8.    2.    5.    0.
New GA best: FIT=   40.436604 SOL=    6.    6.    1.    3.    0.
New GA best: FIT=   97.547842 SOL=    6.    5.    1.    3.    0.
New GA best: FIT=   99.998600 SOL=    8.    9.    1.    1.    0.
========== Genetic Algorithm Best ==========
C:  8, H:  9, O:  1, N:  1, S:  0
Formula: C 8  H 9  O 1  N 1  S 0
Calculated mass:   135.068414
Target mass:       135.068400
Difference:          0.000014
Fitness:            99.998600
 Nitrogen rule: odd mass, odd N atoms - OK.
============================================
 Starting Simulated Annealing optimization...
========= Simulated Annealing Best =========
C:  8, H:  9, O:  1, N:  1, S:  0
Formula: C 8  H 9  O 1  N 1  S 0
Calculated mass:   135.068414
Target mass:       135.068400
Difference:          0.000014
Fitness:            99.998600
 Nitrogen rule: odd mass, odd N atoms - OK.
============================================
=========== Final Best Solution ============
C:  8, H:  9, O:  1, N:  1, S:  0
Formula: C 8  H 9  O 1  N 1  S 0
Calculated mass:   135.068414
Target mass:       135.068400
Difference:          0.000014
Fitness:            99.998600
 Nitrogen rule: odd mass, odd N atoms - OK.
============================================
 Program completed.
Note: The following floating-point exceptions are signalling: IEEE_UNDERFLOW_FLAG IEEE_DENORMAL
```


# A. 更换软件源为清华大学镜像站
## A.1 Ubuntu 24.04.2 LTS 软件源配置
### 代码 A.1.1
```
user1@host:~$ lsb_release -a
No LSB modules are available.
Distributor ID: Ubuntu
Description:    Ubuntu 24.04.2 LTS
Release:        24.04
Codename:       noble
```

### 代码 A.1.2
```
user1@host:~$ sudo vim /etc/apt/sources.list.d/ubuntu.sources
```

### 代码 A.1.3
```
Types: deb
URIs: https://mirrors.tuna.tsinghua.edu.cn/ubuntu
Suites: noble noble-updates noble-backports
Components: main restricted universe multiverse
Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg

# 默认注释了源码镜像以提高 apt update 速度，如有需要可自行取消注释
# Types: deb-src
# URIs: https://mirrors.tuna.tsinghua.edu.cn/ubuntu
# Suites: noble noble-updates noble-backports
# Components: main restricted universe multiverse
# Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg

# 以下安全更新软件源包含了官方源与镜像站配置，如有需要可自行修改注释切换
Types: deb
URIs: http://security.ubuntu.com/ubuntu/
Suites: noble-security
Components: main restricted universe multiverse
Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg

# Types: deb-src
# URIs: http://security.ubuntu.com/ubuntu/
# Suites: noble-security
# Components: main restricted universe multiverse
# Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg

# 预发布软件源，不建议启用

# Types: deb
# URIs: https://mirrors.tuna.tsinghua.edu.cn/ubuntu
# Suites: noble-proposed
# Components: main restricted universe multiverse
# Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg

# # Types: deb-src
# # URIs: https://mirrors.tuna.tsinghua.edu.cn/ubuntu
# # Suites: noble-proposed
# # Components: main restricted universe multiverse
# # Signed-By: /usr/share/keyrings/ubuntu-archive-keyring.gpg
```

### 代码 A.1.4
```
user1@host:~$ sudo apt-get update
```

## A.2 更早或更新版本软件源配置
暂无本小节代码块。


# B. 与Window宿主机共享文件夹
## B.1 WSL子系统
### 代码 B.1.1
```
user1@host:~$ cd /mnt/c
user1@host:/mnt/c$ ls
Users  Program Files  Program Files (x86)  Windows ...
user1@host:~$ cd /mnt/d
```

## B.2 虚拟机
### 代码 B.2.1
```
user1@host:~$ vmware-hgfsclient
```

### 代码 B.2.2
```
user1@host:~$ sudo /usr/bin/vmhgfs-fuse .host:/ /mnt/hgfs -o allow_other -o uid=1000 -o gid=1000 -o umask=022
```

### 代码 B.2.3
```
user1@host:~$ cd /mnt/hgfs
user1@host:/mnt/hgfs$ ls
SharedFolder1  SharedFolder2  ...
```

### 代码 B.2.4
```
user1@host:~$ sudo vim /etc/fstab
```

### 代码 B.2.5
```
.host:/ /mnt/hgfs fuse.vmhgfs-fuse allow_other,uid=1000,gid=1000,umask=022 0 0
```


# C. 程序实例代码
## C.1 计算分子式程序
### 代码 C.1.1
```
      PROGRAM MAIN
C     
C     ========== 数组声明（必须放在可执行语句之前）==========
      DIMENSION SOL_INIT(5)
      DIMENSION GA_RES(5)
      DIMENSION SA_RES(5)
      DIMENSION FINAL_RES(5)
      DIMENSION HIST_FIT(1)
C     =======================================================
      
C     原子量定义（实型）
      DCM = 12.000000
      DHM = 1.007825
      DOM = 15.994915
      DNM = 14.003074
      DSM = 31.972072
      
C     用户输入目标分子量（实型）
      WRITE(*,*) 'Target molecular weight: '
      READ(*,*) TARGET_MASS
      
C     用户输入目标不饱和度（实型）
      WRITE(*,*) 'Minimal degree of unsaturation (e.g., 4.0): '
      READ(*,*) TARGET_UNSAT
      
C     约束参数
      NRULE = 1          ! 1=启用氮规则惩罚，0=禁用（建议启用）
      
C     ==================== 算法选择配置 ====================
      IGA = 1            ! 1=运行遗传算法, 0=跳过
      ISA = 1            ! 1=运行模拟退火, 0=跳过
C     ======================================================
      
C     ============ 原子数量限制配置（整型变量）=============
      ICMIN = 1
      ICMAX = 31
      IHMIN = 0
      IHMAX = 31
      IOMIN = 0
      IOMAX = 31
      INMIN = 0
      INMAX = 31
      ISMIN = 0
      ISMAX = 0
C     ======================================================
      
C     ==================== 遗传算法 ====================
      IF (IGA .EQ. 1) THEN
          WRITE(*,*) 'Starting Genetic Algorithm optimization...'
C         遗传算法子程序（传递目标不饱和度）
          CALL RUN_GA(TARGET_MASS, TARGET_UNSAT,
     +                ICMIN, ICMAX, IHMIN, IHMAX,
     +                IOMIN, IOMAX, INMIN, INMAX, ISMIN, ISMAX,
     +                DCM, DHM, DOM, DNM, DSM, NRULE,
     +                GA_RES, FIT_GA, BEST_INDEX, GA_TIME)
          
C         解码遗传算法结果
          X1_GA = GA_RES(1)
          X2_GA = GA_RES(2)
          X3_GA = GA_RES(3)
          X4_GA = GA_RES(4)
          X5_GA = GA_RES(5)
          CALC_MASS_GA = X1_GA*DCM + X2_GA*DHM + X3_GA*DOM + X4_GA*DNM
     +                 + X5_GA*DSM
          
C         输出遗传算法结果
          WRITE(*,10) '========== Genetic Algorithm Best =========='
          WRITE(*,20) 'C: ', INT(X1_GA), ', H: ', INT(X2_GA),
     +                ', O: ', INT(X3_GA), ', N: ', INT(X4_GA),
     +                ', S: ', INT(X5_GA)
          CALL PRINT_CHEM(INT(X1_GA), INT(X2_GA), INT(X3_GA),
     +                    INT(X4_GA), INT(X5_GA))
          WRITE(*,30) 'Calculated mass: ', CALC_MASS_GA
          WRITE(*,30) 'Target mass:     ', TARGET_MASS
          WRITE(*,30) 'Difference:      ', ABS(TARGET_MASS 
     +                - CALC_MASS_GA)
          WRITE(*,30) 'Fitness:         ', FIT_GA
          
C         检查氮规则
          IROUND_GA = NINT(CALC_MASS_GA)
          CALL CHECK_N_RULE(IROUND_GA, INT(X4_GA))
          
          WRITE(*,10) '============================================'

C         将遗传算法结果作为退火初始解
          DO I = 1, 5
              SOL_INIT(I) = GA_RES(I)
          END DO
      ELSE
          WRITE(*,*) 'Skipping GA, generating random initial ',
     +               'solution...'
C         随机生成满足原子限制的初始解
          CALL RAND_SOL(ICMIN, ICMAX, IHMIN, IHMAX,
     +                  IOMIN, IOMAX, INMIN, INMAX,
     +                  ISMIN, ISMAX, SOL_INIT)
C         计算随机解的适应度（传递目标不饱和度）
          CALL FIT_FUNC(INT(SOL_INIT(1)), INT(SOL_INIT(2)),
     +                  INT(SOL_INIT(3)), INT(SOL_INIT(4)),
     +                  INT(SOL_INIT(5)), TARGET_MASS, TARGET_UNSAT,
     +                  DCM, DHM, DOM, DNM, DSM, NRULE,
     +                  FIT_RAND)
          
          WRITE(*,20) 'Random initial: C', INT(SOL_INIT(1)),
     +                ' H', INT(SOL_INIT(2)),
     +                ' O', INT(SOL_INIT(3)),
     +                ' N', INT(SOL_INIT(4)),
     +                ' S', INT(SOL_INIT(5))
          WRITE(*,30) 'Fitness: ', FIT_RAND
      END IF
      
C     ==================== 模拟退火算法 ====================
      IF (ISA .EQ. 1) THEN
          WRITE(*,*) 'Starting Simulated Annealing optimization...'
          
C         模拟退火参数
          T_INIT = 10000.0
          T_FINAL = 1.0E-3
          ALPHA = 0.99
          IMAX_ITER = 2000    ! 整型变量
          
C         使用遗传算法结果或随机解作为初始解（传递目标不饱和度）
          CALL RUN_SA(SOL_INIT, TARGET_MASS, TARGET_UNSAT,
     +                ICMIN, ICMAX, IHMIN, IHMAX,
     +                IOMIN, IOMAX, INMIN, INMAX, ISMIN, ISMAX,
     +                T_INIT, T_FINAL, ALPHA, IMAX_ITER,
     +                DCM, DHM, DOM, DNM, DSM, NRULE,
     +                SA_RES, FIT_SA, SA_TIME, HIST_FIT)
          
C         解码模拟退火结果
          X1_SA = SA_RES(1)
          X2_SA = SA_RES(2)
          X3_SA = SA_RES(3)
          X4_SA = SA_RES(4)
          X5_SA = SA_RES(5)
          CALC_MASS_SA = X1_SA*DCM + X2_SA*DHM + X3_SA*DOM + X4_SA*DNM
     +                 + X5_SA*DSM
          
          WRITE(*,10) '========= Simulated Annealing Best ========='
          WRITE(*,20) 'C: ', INT(X1_SA), ', H: ', INT(X2_SA),
     +                ', O: ', INT(X3_SA), ', N: ', INT(X4_SA),
     +                ', S: ', INT(X5_SA)
          CALL PRINT_CHEM(INT(X1_SA), INT(X2_SA), INT(X3_SA),
     +                    INT(X4_SA), INT(X5_SA))
          WRITE(*,30) 'Calculated mass: ', CALC_MASS_SA
          WRITE(*,30) 'Target mass:     ', TARGET_MASS
          WRITE(*,30) 'Difference:      ', ABS(TARGET_MASS 
     +                - CALC_MASS_SA)
          WRITE(*,30) 'Fitness:         ', FIT_SA
          
          IROUND_SA = NINT(CALC_MASS_SA)
          CALL CHECK_N_RULE(IROUND_SA, INT(X4_SA))
          
          WRITE(*,10) '============================================'


C         最终结果使用模拟退火结果
          DO I = 1, 5
              FINAL_RES(I) = SA_RES(I)
          END DO
          FIT_FINAL = FIT_SA
      ELSE
          IF (IGA .EQ. 1) THEN
              DO I = 1, 5
                  FINAL_RES(I) = GA_RES(I)
              END DO
              FIT_FINAL = FIT_GA
          ELSE
              DO I = 1, 5
                  FINAL_RES(I) = SOL_INIT(I)
              END DO
              FIT_FINAL = FIT_RAND
          END IF
      END IF
      
C     ==================== 最终结果输出 ====================
      X1 = FINAL_RES(1)
      X2 = FINAL_RES(2)
      X3 = FINAL_RES(3)
      X4 = FINAL_RES(4)
      X5 = FINAL_RES(5)
      CALC_MASS = X1*DCM + X2*DHM + X3*DOM + X4*DNM + X5*DSM
      
      WRITE(*,10) '=========== Final Best Solution ============'
      WRITE(*,20) 'C: ', INT(X1), ', H: ', INT(X2),
     +            ', O: ', INT(X3), ', N: ', INT(X4),
     +            ', S: ', INT(X5)
      CALL PRINT_CHEM(INT(X1), INT(X2), INT(X3),
     +                INT(X4), INT(X5))
      WRITE(*,30) 'Calculated mass: ', CALC_MASS
      WRITE(*,30) 'Target mass:     ', TARGET_MASS
      WRITE(*,30) 'Difference:      ', ABS(TARGET_MASS - CALC_MASS)
      WRITE(*,30) 'Fitness:         ', FIT_FINAL
      
      IROUND = NINT(CALC_MASS)
      CALL CHECK_N_RULE(IROUND, INT(X4))
      
      WRITE(*,10) '============================================'


C     保存结果到文件
      CALL SAVE_RES(TARGET_MASS, FINAL_RES, CALC_MASS)
      
      WRITE(*,*) 'Program completed.'
      
10    FORMAT(A)
20    FORMAT(A,I2,A,I2,A,I2,A,I2,A,I2)
30    FORMAT(A,F12.6)
      
      STOP
      END
      
C     *********************************************************
C     子程序：随机生成初始解
C     输入：各原子数量限制（整型），输出：5维实型数组SOL
C     *********************************************************
      SUBROUTINE RAND_SOL(ICMIN, ICMAX, IHMIN, IHMAX,
     +                    IOMIN, IOMAX, INMIN, INMAX,
     +                    ISMIN, ISMAX, SOL)
      
      DIMENSION SOL(5)
      
C     初始化随机数生成器（Fortran90特性）
      CALL RANDOM_SEED()
      
      CALL RANDOM_NUMBER(R1)
      SOL(1) = INT(R1 * (ICMAX - ICMIN + 1)) + ICMIN
      
      CALL RANDOM_NUMBER(R2)
      SOL(2) = INT(R2 * (IHMAX - IHMIN + 1)) + IHMIN
      
      CALL RANDOM_NUMBER(R3)
      SOL(3) = INT(R3 * (IOMAX - IOMIN + 1)) + IOMIN
      
      CALL RANDOM_NUMBER(R4)
      SOL(4) = INT(R4 * (INMAX - INMIN + 1)) + INMIN
      
      CALL RANDOM_NUMBER(R5)
      SOL(5) = INT(R5 * (ISMAX - ISMIN + 1)) + ISMIN
      
      RETURN
      END
      
C     *********************************************************
C     适应度函数（改进版）
C     输入：原子数（整型）、目标质量、目标不饱和度、原子量、
C           氮规则开关（NRULE）
C     输出：适应度（实型，值越大越好）
C     *********************************************************
      SUBROUTINE FIT_FUNC(IC, IH, IO, IN, IS, 
     +                    TARGET_MASS, TARGET_UNSAT,
     +                    DCM, DHM, DOM, DNM, DSM, NRULE,
     +                    FITNESS)
      
C     计算分子量
      CALC_MASS = IC*DCM + IH*DHM + IO*DOM + IN*DNM + IS*DSM
      
C     基础适应度：与目标质量越接近，适应度越高
      DIF_M = ABS(CALC_MASS - TARGET_MASS)
      FITNESS = 100.0 / (DIF_M + 1.0)
      
C     ---------- 不饱和度惩罚（使用用户输入的目标值）----------
C     不饱和度 = (2*C + 2 + N - H) / 2.0 （忽略硫的影响）
      IF ((2.0*IC + 2.0 + IN - IH) / 2.0 .LT. TARGET_UNSAT) THEN
          FITNESS = FITNESS - 5.0
      END IF
      
C     ---------- 氮规则惩罚（若启用）----------
      IF (NRULE .EQ. 1) THEN
          IROUND = NINT(CALC_MASS)
          IEVEN = MOD(IROUND, 2)      ! 0为偶数，1为奇数
          N_EVEN = MOD(IN, 2)         ! 0为偶数，1为奇数
C         规则：若N为奇数，分子量应为奇数；若N为偶数，分子量应为偶数
          IF ((IEVEN .EQ. 0 .AND. N_EVEN .NE. 0) .OR.
     +        (IEVEN .NE. 0 .AND. N_EVEN .EQ. 0)) THEN
              FITNESS = FITNESS - 10.0  ! 加性惩罚，适应度降低10
          END IF
      END IF
      
C     ---------- 氢原子合理性惩罚（防止完全不饱和）----------
C     参考MATLAB：若 H > 2*C + N + 2，则不合理，给予惩罚
C     IF (IH .GT. 2*IC + IN + 2) THEN
C         FITNESS = FITNESS - 5.0
C     END IF
      
C     确保适应度不为负（至少为一个小正数）
      IF (FITNESS .LT. 0.01) FITNESS = 0.01
      
      RETURN
      END
      
C     *********************************************************
C     打印化学式
C     输入：各原子数（整型）
C     *********************************************************
      SUBROUTINE PRINT_CHEM(IC, IH, IO, IN, IS)
      
C     输出格式：例如 C6H12O6
      WRITE(*,100)
     +'Formula: C', IC, '  H', IH, '  O', IO, '  N', IN, '  S', IS
100   FORMAT(A,I2,A,I2,A,I2,A,I2,A,I2)
      
      RETURN
      END
      
C     *********************************************************
C     检查氮规则并输出结果
C     输入：取整后的分子量（整型），氮原子数（整型）
C     *********************************************************
      SUBROUTINE CHECK_N_RULE(IROUND_MASS, N_ATOM)
      
      IEVEN = MOD(IROUND_MASS, 2)
      N_EVEN = MOD(N_ATOM, 2)
      
      IF (IEVEN .EQ. 0 .AND. N_EVEN .EQ. 0) THEN
          WRITE(*,*) 'Nitrogen rule: even mass, even N atoms - OK.'
      ELSE IF (IEVEN .NE. 0 .AND. N_EVEN .NE. 0) THEN
          WRITE(*,*) 'Nitrogen rule: odd mass, odd N atoms - OK.'
      ELSE
          WRITE(*,*) 'Nitrogen rule: mass/N parity mismatch - ',
     +               'may violate nitrogen rule!'
      END IF
      
      RETURN
      END
      
C     *********************************************************
C     保存结果到文件
C     输入：目标质量、最终解数组、计算分子量
C     *********************************************************
      SUBROUTINE SAVE_RES(TARGET_MASS, FINAL_RES, CALC_MASS)
      
      DIMENSION FINAL_RES(5)
      
      OPEN(UNIT=10, FILE='cal_result.txt', STATUS='UNKNOWN', 
     +     POSITION='APPEND')
      WRITE(10,'(A20,F15.6)') 'Target mass: ', TARGET_MASS
      WRITE(10,'(A20)') 'Best solution:'
      WRITE(10,'(A20,I15)') 'C: ', INT(FINAL_RES(1))
      WRITE(10,'(A20,I15)') 'H: ', INT(FINAL_RES(2))
      WRITE(10,'(A20,I15)') 'O: ', INT(FINAL_RES(3))
      WRITE(10,'(A20,I15)') 'N: ', INT(FINAL_RES(4))
      WRITE(10,'(A20,I15)') 'S: ', INT(FINAL_RES(5))
      WRITE(10,'(A20,F15.6)') 'Calculated mass: ', CALC_MASS
      WRITE(10,'(A20,F15.6,/)')
     +'Difference: ', ABS(TARGET_MASS - CALC_MASS)
      CLOSE(10)
      
      RETURN
      END
      
C     *********************************************************
C     遗传算法主程序
C     *********************************************************
      SUBROUTINE RUN_GA(TARGET_MASS, TARGET_UNSAT,
     +                  ICMIN, ICMAX, IHMIN, IHMAX,
     +                  IOMIN, IOMAX, INMIN, INMAX,
     +                  ISMIN, ISMAX,
     +                  DCM, DHM, DOM, DNM, DSM, NRULE,
     +                  BEST_SOL, BEST_FIT, BEST_INDEX, TIME)
      
      DIMENSION BEST_SOL(5)
      DIMENSION POP(500,5), FIT(500), NEWPOP(500,5)
      DIMENSION TEMP(5)   ! 实型数组，用于存储随机解
      DIMENSION BEST_SOL_GLOBAL(5)      ! 新增：全局最优解数组

      
C     遗传算法参数
      IPOPS = 500        ! 种群大小
      IMAXGEN = 10000    ! 最大代数
      PCROSS = 0.8       ! 交叉概率（实型）
      PMUT = 0.3         ! 变异概率（实型）
      
C     初始化种群
      DO I = 1, IPOPS
          CALL RAND_SOL(ICMIN, ICMAX, IHMIN, IHMAX,
     +                  IOMIN, IOMAX, INMIN, INMAX,
     +                  ISMIN, ISMAX, TEMP)
          DO J = 1, 5
              POP(I,J) = TEMP(J)
          END DO
      END DO
      
C     初始化全局最优
      BEST_FIT_GLOBAL = -1.0E10
      
C     主循环
      DO IGEN = 1, IMAXGEN
C         计算适应度
          DO I = 1, IPOPS
              CALL FIT_FUNC(INT(POP(I,1)), INT(POP(I,2)),
     +                      INT(POP(I,3)), INT(POP(I,4)),
     +                      INT(POP(I,5)), TARGET_MASS, TARGET_UNSAT,
     +                      DCM, DHM, DOM, DNM, DSM, NRULE,
     +                      FIT(I))
          END DO
          
C         寻找当前代最优个体
          BEST = -1.0E10
          DO I = 1, IPOPS
              IF (FIT(I) .GT. BEST) THEN
                  BEST = FIT(I)
                  IBEST = I
              END IF
          END DO
          
C         保留最优个体（精英策略）
          DO J = 1, 5
              BEST_SOL(J) = POP(IBEST,J)
          END DO
          BEST_FIT = BEST
          BEST_INDEX = IBEST
          
C         更新全局最优
          IF (BEST .GT. BEST_FIT_GLOBAL) THEN
              BEST_FIT_GLOBAL = BEST
              DO J = 1, 5
                  BEST_SOL_GLOBAL(J) = POP(IBEST,J)
              END DO
              WRITE(*,'(A,F12.6,A,5F6.0)') 'New GA best: FIT=', 
     +        BEST_FIT_GLOBAL,' SOL=', (BEST_SOL_GLOBAL(J), J=1,5)
C         ============ 质量差 < 0.00001 时跳出 ============
C          计算当前全局最优解的分子量
              CALC_MASS_TMP = BEST_SOL_GLOBAL(1)*DCM 
     +                      + BEST_SOL_GLOBAL(2)*DHM
     +                      + BEST_SOL_GLOBAL(3)*DOM
     +                      + BEST_SOL_GLOBAL(4)*DNM
     +                      + BEST_SOL_GLOBAL(5)*DSM
              DIF_MASS = ABS(CALC_MASS_TMP - TARGET_MASS)
              IF (DIF_MASS .LT. 0.00001) THEN
                  WRITE(*,*) 'GA: Mass difference < 0.00001, ',
     +                       'terminating early.'
                  GOTO 999   ! 直接跳出主循环
              END IF
C         ================================================
          END IF
          
C         选择（轮盘赌）
          SUMFIT = 0.0
          DO I = 1, IPOPS
              SUMFIT = SUMFIT + FIT(I)
          END DO
          
          DO I = 1, IPOPS
              CALL RANDOM_NUMBER(R)
              SELECT = R * SUMFIT
              PARTIAL = 0.0
              DO K = 1, IPOPS
                  PARTIAL = PARTIAL + FIT(K)
                  IF (PARTIAL .GE. SELECT) THEN
                      DO J = 1, 5
                          NEWPOP(I,J) = POP(K,J)
                      END DO
                      GOTO 100
                  END IF
              END DO
100           CONTINUE
          END DO
          
C         交叉（单点交叉）
          DO I = 1, IPOPS, 2
              CALL RANDOM_NUMBER(R)
              IF (R .LT. PCROSS) THEN
                  IPOS = INT(R * 4) + 1   ! 交叉点1-4
                  DO J = IPOS, 5
                      TEMP_VAL = NEWPOP(I,J)
                      NEWPOP(I,J) = NEWPOP(I+1,J)
                      NEWPOP(I+1,J) = TEMP_VAL
                  END DO
              END IF
          END DO
          
C         交叉后边界检查：确保每个个体在原子限制范围内
          DO I = 1, IPOPS
              IF (NEWPOP(I,1) .LT. ICMIN) NEWPOP(I,1) = ICMIN
              IF (NEWPOP(I,1) .GT. ICMAX) NEWPOP(I,1) = ICMAX
              IF (NEWPOP(I,2) .LT. IHMIN) NEWPOP(I,2) = IHMIN
              IF (NEWPOP(I,2) .GT. IHMAX) NEWPOP(I,2) = IHMAX
              IF (NEWPOP(I,3) .LT. IOMIN) NEWPOP(I,3) = IOMIN
              IF (NEWPOP(I,3) .GT. IOMAX) NEWPOP(I,3) = IOMAX
              IF (NEWPOP(I,4) .LT. INMIN) NEWPOP(I,4) = INMIN
              IF (NEWPOP(I,4) .GT. INMAX) NEWPOP(I,4) = INMAX
              IF (NEWPOP(I,5) .LT. ISMIN) NEWPOP(I,5) = ISMIN
              IF (NEWPOP(I,5) .GT. ISMAX) NEWPOP(I,5) = ISMAX
          END DO
          
C         变异（均匀变异）
          DO I = 1, IPOPS
              DO J = 1, 5
                  CALL RANDOM_NUMBER(R)
                  IF (R .LT. PMUT) THEN
C                     根据原子范围随机重置
                      IF (J .EQ. 1) THEN
                          CALL RANDOM_NUMBER(R1)
                          NEWPOP(I,J) = INT(R1 * (ICMAX-ICMIN+1))
     +                                + ICMIN
                      ELSE IF (J .EQ. 2) THEN
                          CALL RANDOM_NUMBER(R1)
                          NEWPOP(I,J) = INT(R1 * (IHMAX-IHMIN+1))
     +                                + IHMIN
                      ELSE IF (J .EQ. 3) THEN
                          CALL RANDOM_NUMBER(R1)
                          NEWPOP(I,J) = INT(R1 * (IOMAX-IOMIN+1))
     +                                + IOMIN
                      ELSE IF (J .EQ. 4) THEN
                          CALL RANDOM_NUMBER(R1)
                          NEWPOP(I,J) = INT(R1 * (INMAX-INMIN+1))
     +                                + INMIN
                      ELSE
                          CALL RANDOM_NUMBER(R1)
                          NEWPOP(I,J) = INT(R1 * (ISMAX-ISMIN+1))
     +                                + ISMIN
                      END IF
                  END IF
              END DO
          END DO
          
C         精英保留：将当前代最优个体放入下一代第一个位置
          DO J = 1, 5
              NEWPOP(1,J) = BEST_SOL(J)
          END DO
          
C         更新种群
          DO I = 1, IPOPS
              DO J = 1, 5
                  POP(I,J) = NEWPOP(I,J)
              END DO
          END DO
          
      END DO

999   CONTINUE   ! 提前跳出时直接到达此处
      
C     返回全局最优解（而非最后一代最优）
      DO J = 1, 5
          BEST_SOL(J) = BEST_SOL_GLOBAL(J)
      END DO
      BEST_FIT = BEST_FIT_GLOBAL
      
C     记录时间（简单设为0.0）
      TIME = 0.0
      
      RETURN
      END
      
C     *********************************************************
C     模拟退火算法主程序
C     *********************************************************
      SUBROUTINE RUN_SA(SOL_INIT, TARGET_MASS, TARGET_UNSAT,
     +                  ICMIN, ICMAX, IHMIN, IHMAX,
     +                  IOMIN, IOMAX, INMIN, INMAX,
     +                  ISMIN, ISMAX,
     +                  T_INIT, T_FINAL, ALPHA, IMAX_ITER,
     +                  DCM, DHM, DOM, DNM, DSM, NRULE,
     +                  BEST_SOL, BEST_FIT, TIME, HIST_FIT)
      
      DIMENSION SOL_INIT(5), BEST_SOL(5)
      DIMENSION CURR_SOL(5), SOL_NEW(5)
      DIMENSION HIST_FIT(1)      ! 未使用，仅占位
      
C     初始化解
      DO I = 1, 5
          CURR_SOL(I) = SOL_INIT(I)
      END DO
      
      CALL FIT_FUNC(INT(CURR_SOL(1)), INT(CURR_SOL(2)),
     +              INT(CURR_SOL(3)), INT(CURR_SOL(4)),
     +              INT(CURR_SOL(5)), TARGET_MASS, TARGET_UNSAT,
     +              DCM, DHM, DOM, DNM, DSM, NRULE,
     +              FIT_CURR)
      
      DO I = 1, 5
          BEST_SOL(I) = CURR_SOL(I)
      END DO
      BEST_FIT = FIT_CURR
      
      TEMP = T_INIT
      
C     退火主循环
      DO WHILE (TEMP .GT. T_FINAL)
          DO ITER = 1, IMAX_ITER
C             【改进】自适应邻域生成（模拟MATLAB逻辑）
C             根据当前温度与初始温度的比例确定扰动步长
              TEMP_RATIO = TEMP / T_INIT
C             步长范围：高温时最大可达5，低温时最小为1
              STEP = MAX(1, INT(TEMP_RATIO * 5.0 + 0.5))
              
C             随机选择要变动的原子数量（1~3个）
              CALL RANDOM_NUMBER(R)
              NDIM = INT(R * 3.0) + 1
              
C             复制当前解到新解
              DO I = 1, 5
                  SOL_NEW(I) = CURR_SOL(I)
              END DO
              
C             对选中的原子进行扰动
              DO ID = 1, NDIM
                  CALL RANDOM_NUMBER(R)
                  IATOM = INT(R * 5.0) + 1   ! 1~5
                  
C                 决定变化方向（+或-）
                  CALL RANDOM_NUMBER(R)
                  IF (R .LT. 0.5) THEN
                      DELTA = STEP
                  ELSE
                      DELTA = -STEP
                  END IF
                  
                  IF (IATOM .EQ. 1) THEN
                      NEW_VAL = CURR_SOL(1) + DELTA
                      IF (NEW_VAL .GE. ICMIN .AND.
     +                    NEW_VAL .LE. ICMAX) SOL_NEW(1) = NEW_VAL
                  ELSE IF (IATOM .EQ. 2) THEN
                      NEW_VAL = CURR_SOL(2) + DELTA
                      IF (NEW_VAL .GE. IHMIN .AND.
     +                    NEW_VAL .LE. IHMAX) SOL_NEW(2) = NEW_VAL
                  ELSE IF (IATOM .EQ. 3) THEN
                      NEW_VAL = CURR_SOL(3) + DELTA
                      IF (NEW_VAL .GE. IOMIN .AND.
     +                    NEW_VAL .LE. IOMAX) SOL_NEW(3) = NEW_VAL
                  ELSE IF (IATOM .EQ. 4) THEN
                      NEW_VAL = CURR_SOL(4) + DELTA
                      IF (NEW_VAL .GE. INMIN .AND.
     +                    NEW_VAL .LE. INMAX) SOL_NEW(4) = NEW_VAL
                  ELSE
                      NEW_VAL = CURR_SOL(5) + DELTA
                      IF (NEW_VAL .GE. ISMIN .AND.
     +                    NEW_VAL .LE. ISMAX) SOL_NEW(5) = NEW_VAL
                  END IF
              END DO
              
C             额外：以20%概率进行完全随机重置（大扰动，增加多样性）
              CALL RANDOM_NUMBER(R)
              IF (R .LT. 0.2) THEN
C                 随机选择1~2个维度完全重置
                  CALL RANDOM_NUMBER(R2)
                  NRST = INT(R2 * 2.0) + 1
                  DO IR = 1, NRST
                      CALL RANDOM_NUMBER(R3)
                      IATOM_RST = INT(R3 * 5.0) + 1
                      IF (IATOM_RST .EQ. 1) THEN
                          CALL RANDOM_NUMBER(R4)
                          SOL_NEW(1) = INT(R4 * (ICMAX-ICMIN+1)) 
     +                               + ICMIN
                      ELSE IF (IATOM_RST .EQ. 2) THEN
                          CALL RANDOM_NUMBER(R4)
                          SOL_NEW(2) = INT(R4 * (IHMAX-IHMIN+1)) 
     +                               + IHMIN
                      ELSE IF (IATOM_RST .EQ. 3) THEN
                          CALL RANDOM_NUMBER(R4)
                          SOL_NEW(3) = INT(R4 * (IOMAX-IOMIN+1)) 
     +                               + IOMIN
                      ELSE IF (IATOM_RST .EQ. 4) THEN
                          CALL RANDOM_NUMBER(R4)
                          SOL_NEW(4) = INT(R4 * (INMAX-INMIN+1)) 
     +                               + INMIN
                      ELSE
                          CALL RANDOM_NUMBER(R4)
                          SOL_NEW(5) = INT(R4 * (ISMAX-ISMIN+1)) 
     +                               + ISMIN
                      END IF
                  END DO
              END IF
              
C             计算新适应度
              CALL FIT_FUNC(INT(SOL_NEW(1)), INT(SOL_NEW(2)),
     +                      INT(SOL_NEW(3)), INT(SOL_NEW(4)),
     +                      INT(SOL_NEW(5)), TARGET_MASS, TARGET_UNSAT,
     +                      DCM, DHM, DOM, DNM, DSM, NRULE,
     +                      FIT_NEW)
              
              DELTA_FIT = FIT_NEW - FIT_CURR
              
              IF (DELTA_FIT .GT. 0.0) THEN
C                 接受更优解
                  DO I = 1, 5
                      CURR_SOL(I) = SOL_NEW(I)
                  END DO
                  FIT_CURR = FIT_NEW
C                 更新全局最优
                  IF (FIT_NEW .GT. BEST_FIT) THEN
                      BEST_FIT = FIT_NEW
                      DO I = 1, 5
                          BEST_SOL(I) = SOL_NEW(I)
                      END DO
                      WRITE(*,'(A,F12.6,A,5F6.0)') 'New SA best: FIT=', 
     +                BEST_FIT,' SOL=', (BEST_SOL(J), J=1,5)

C         ============ 质量差 < 0.00001 时跳出 ============
                      CALC_MASS_TMP = BEST_SOL(1)*DCM 
     +                              + BEST_SOL(2)*DHM
     +                              + BEST_SOL(3)*DOM
     +                              + BEST_SOL(4)*DNM
     +                              + BEST_SOL(5)*DSM
                      DIF_MASS = ABS(CALC_MASS_TMP - TARGET_MASS)
                      IF (DIF_MASS .LT. 0.00001) THEN
                          WRITE(*,*) 'SA: Mass difference < 0.00001, ',
     +                               'terminating annealing.'
                          TEMP = T_FINAL - 1.0   ! 强制外层循环条件为假
                          EXIT                    ! 跳出内层循环
                      END IF
C         ================================================

                  END IF
              ELSE
C                 以概率接受劣化解
                  CALL RANDOM_NUMBER(R)
                  IF (R .LT. EXP(DELTA_FIT / TEMP)) THEN
                      DO I = 1, 5
                          CURR_SOL(I) = SOL_NEW(I)
                      END DO
                      FIT_CURR = FIT_NEW
                  END IF
              END IF
          END DO
C         降温
          TEMP = TEMP * ALPHA
      END DO
      
      TIME = 0.0
      
      RETURN
      END
```


