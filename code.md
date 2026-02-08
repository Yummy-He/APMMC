由AI从文档中提取的代码块，在这里可以方便地复制：

---

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
### 代码 0.2.3  
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

---

# 1. Linux入门  
## 1.1 Linux简介  
### 代码 1.1.1  
```
user1@host:~$ lsb_release -a  
No LSB modules are available.  
Distributor ID: Ubuntu  
Description:    Ubuntu 24.04.2 LTS  
Release:        24.04  
Codename:       noble  
```  

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
user1@host:~$ pwd | ls  
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
user1@host:~$ vim test/grades.txt  
```  

## 1.10 与window宿主机共享文件  
暂无本小节代码块。  

---

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

---

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

---

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
C SUBROUTINE TO SWAP TWO NUMBERS  
      SUBROUTINE SWAP(A, B)  
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

## 4.2 程序框图  
暂无本小节代码块。  

## 4.3 IF语句  
### 代码 4.3.1  
```
      IF(X.GT.0) WRITE(6,*)X,Y  
```  
### 代码 4.3.2  
```
      IF(X.GT.0) THEN  
          Y = X**2  
          WRITE(6,*)Y  
      ENDIF  
```  
### 代码 4.3.3  
```
      IF(X.GT.0) THEN  
          IF(Y.LT.0) THEN  
              Z = X + Y  
          ELSE  
              Z = X - Y  
          ENDIF  
      ENDIF  
```  
### 代码 4.3.4  
```
      IF(X) 10, 20, 30  
10    WRITE(6,*) 'X < 0'  
20    WRITE(6,*) 'X = 0'  
30    WRITE(6,*) 'X > 0'  
```  
### 代码 4.3.5  
```
      IF(ABS(X - TARGET).LT..00001) THEN  
          ...  
      ENDIF  
```  

## 4.4 GOTO语句  
### 代码 4.4.1  
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
### 代码 4.4.2  
```
      INTEGER I  
      I = 1  
10    IF(I.GT.100) GOTO 20  
      I = I + 1  
      GOTO 10  
20    END  
```  
### 代码 4.4.3  
```
      GOTO (10, 20, 30) N  
10    WRITE(6,*) 'N = 1'  
20    WRITE(6,*) 'N = 2'  
30    WRITE(6,*) 'N = 3'  
      END  
```  

## 4.5 DO循环语句  
### 代码 4.5.1  
```
      DO LABEL VAR = START, END, STEP  
          ! 循环体  
LABEL CONTINUE  
```  
### 代码 4.5.2  
```
      INTEGER I, SUM  
      SUM = 0  
      DO 10 I = 1, 10  
          SUM = SUM + I  
10    CONTINUE  
      WRITE(6,*) '1到10的整数和为：', SUM  
      END  
```  
### 代码 4.5.3  
```
      INTEGER I, SUM  
      SUM = 0  
      DO I = 1, 10  
          SUM = SUM + I  
      END DO  
      WRITE(6,*) '1到10的整数和为：', SUM  
      END  
```  
### 代码 4.5.4  
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

---

# 5. 程序实例  
## 5.1 简单程序  
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

## 5.2 复杂程序  
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
### 代码 5.2.3  
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
### 代码 5.2.4  
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
### 代码 5.2.5  
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
### 代码 5.2.6  
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
### 代码 5.2.7  
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
### 代码 5.2.8  
```
user1@host:~$ sudo apt-get install rs  
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 5 5 > matrix1.txt  
```  
### 代码 5.2.9  
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
### 代码 5.2.10  
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
### 代码 5.2.11  
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
### 代码 5.2.12  
```
user1@host:~$ echo "2 3 2" >matrix2.txt  
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 2 3 >> matrix2.txt  
user1@host:~$ shuf -r -n 25 -i 5-10 | rs 3 2 >> matrix2.txt  
```  
### 代码 5.2.13  
```
user1@host:~/examples$ gfortran -o matmult matmult.f  
user1@host:~/examples$ ./matmult < matrix2.txt  
 RESULT MATRIX C:  
        131.0000        133.0000  
        135.0000        128.0000  
```  

---

# A. 更换软件源为清华大学镜像站  
## A.1 Ubuntu 24.04.2 LTS 软件源配置  
### 代码 A.1.1  
```
user1@host:~$ sudo vim /etc/apt/sources.list.d/ubuntu.sources  
```  
### 代码 A.1.2  
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
### 代码 A.1.3  
```
user1@host:~$ sudo apt-get update  
```  

## A.2 更早或更新版本软件源配置  
暂无本小节代码块。  

---

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