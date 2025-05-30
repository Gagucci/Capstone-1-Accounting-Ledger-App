# Capstone One : Accounting Ledger App

```md
             ╔────────────────────────────────────────────────────────────────────────────╗
             │                   ______     ______     ______                             │
             │                  /\  __ \   /\  ___\   /\  ___\                            │
             │                  \ \  __ \  \ \ \____  \ \ \__ \                           │
             │                   \ \_\ \_\  \ \_____\  \ \_____\                          │
             │                    \/_/\/_/   \/_____/   \/_____/                          │
             │                                                                            │
             │ ______     ______     __   __     __  __     __     __   __     ______     │
             │/\  == \   /\  __ \   /\ "-.\ \   /\ \/ /    /\ \   /\ "-.\ \   /\  ___\    │
             │\ \  __<   \ \  __ \  \ \ \-.  \  \ \  _"-.  \ \ \  \ \ \-.  \  \ \ \__ \   │
             │ \ \_____\  \ \_\ \_\  \ \_\\"\_\  \ \_\ \_\  \ \_\  \ \_\\"\_\  \ \_____\  │
             │  \/_____/   \/_/\/_/   \/_/ \/_/   \/_/\/_/   \/_/   \/_/ \/_/   \/_____/  │
             │                                                                            │
             │ ______     __  __     ______     ______   ______     __    __     ______   │
             │/\  ___\   /\ \_\ \   /\  ___\   /\__  _\ /\  ___\   /\ "-./  \   /\  ___\  │
             │\ \___  \  \ \____ \  \ \___  \  \/_/\ \/ \ \  __\   \ \ \-./\ \  \ \___  \ │
             │ \/\_____\  \/\_____\  \/\_____\    \ \_\  \ \_____\  \ \_\ \ \_\  \/\_____\│
             │  \/_____/   \/_____/   \/_____/     \/_/   \/_____/   \/_/  \/_/   \/_____/│
             ╚────────────────────────────────────────────────────────────────────────────╝
```
 


## 🌏 Table of Contents:
- [Description](#description)
- [Installation](#installation)
- [Code Highlight](#code-highlight)
- [Credits and Resources](#credits-and-resources)
- [License](#license)

## Preview:
<img src="./img/app gif.gif">


## Description:
First capstone project for Year Up app development track. A banking application that allows users to add deposits, make payments, view detailed payment history, and generate account reports with specific parameters. A CLI app made fully with java, makes use of fundemental concepts such as CRUD, loops, arraylists, and reading/writing to files.  


## Installation:

* `git clone https://github.com/Gagucci/Capstone-1-Accounting-Ledger-App.git`
* `launch application with Intellij IDE`
* `run program with maven to launch`


## Code Highlight:

For-each loop that converts a string holding the ascii art into a array of characters, then prints each character with a 1 millisecond delay:

``` java

for (char c : art.toCharArray()) {
                    System.out.print(c);
                    Thread.sleep(1); // Adjust the delay (milliseconds) to control speed
                    running = true;
                }
```
<img src ="./img/ascii gif.gif">

For loop that adds equal signs to the loading bar up by however many times i's full value(100) is divisible by the specified amount(100 / 10 = 10, 10 equals signs).\r moves the cursor to print on the same line horizontally as opposed to moving to a new line. 

``` java
public static void loadingBar() throws InterruptedException {
        for (int i = 0; i <= 100; i+=20) {
            System.out.print("\rLoading: [" + "=".repeat(i/10) + "] " + i + "%");
            TimeUnit.MILLISECONDS.sleep(100);
        }
        System.out.println("\n");
    }
```
<img src ="./img/loadbar gif.gif">


## Credits and Resources:
* Assistance from fellow Year Up students.
* Instructor: Ramsey M.
* Pluralsight Workbooks 1-3
* [Java LocalDateTime Documentation](https://docs.oracle.com/en/java/javase/24/docs/api/java.base/java/time/LocalDateTime.html)
* Google search
* DeepSeek and Google Gemini for troubleshooting.
* Source Code by Pluralsight.


## License:
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
