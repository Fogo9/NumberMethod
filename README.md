# **NUMBER METHOD**

# Information

* **According to the value received from the user, a recursive method was written without using a loop.**

# Technologies Used

* **JAVA**

# Contents

* The variables **n** and **total** are defined with int.

* With the recursive method, the result value is decreased by 5 and increased by 5.

<br />

# Codes

```Java

        import java.util.Scanner;

        public class numbermethod{

            public static void main(String[] args) {

                int n;

                Scanner input = new Scanner(System.in);

                System.out.print("Enter The Number : ");

                n = input.nextInt();

                number(n);

            }


```

```Java

            static void number(int n) {

                number(n, 0);

            }

            static int number(int n, int total) {

                if(n <= 0)

                    return result(n, total);

                System.out.print(n + " ");

                return number(n - 5, ++total);
            }

            static int result(int n, int total) {

                System.out.print(n + " ");

                if(total == 0)

                    System.exit(0);

                return result(n + 5, --total);
            }
        }

```

```bash

    Enter The Number : 16
    16 11 6 1 -4 1 6 11 16

    Enter The Number : 10
    10 5 0 5 10

    Enter The Number : 25
    25 20 15 10 5 0 5 10 15 20 25

    Enter The Number : 5
    5 0 5

```

<br />

# LINK

* Click here https://github.com/Fogo9/NumberMethod.git to access the Github page for this project.

<br />

# LICENSE

* This software is licensed By Tuncay Demir under the MIT license.

<br />

>[Patika.dev](https://app.patika.dev/fogomurphy)

<br/>

| Name |  Email |
| ---- |  ----- |
| Tuncay | tuncaydemir682@gmail.com |
