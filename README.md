<header>
<h1 align="center">
  <a href="https://github.com/jdecorte-be/push-swap"><img src=".assets/banner.png" alt="push-swap" ></a>
  push-swap
  <br>
</h1>

<p align="center">
  An algorithm project from 42 school. Sorts a list of integers using two stacks and a limited set of instructions, aiming for the shortest solution.
</p>

<p align="center">
<a href="https://github.com/jdecorte-be/push-swap">
    <img src="https://img.shields.io/badge/Language-C-A8B9CC?logo=c&logoColor=white&labelColor=000000"
         alt="Language C">
  </a>
<a href="https://www.42.fr/">
    <img src="https://img.shields.io/badge/School-42-00BABC?logo=42&logoColor=white&labelColor=000000"
         alt="School 42">
  </a>
<a href="https://github.com/jdecorte-be/push-swap">
    <img src="https://img.shields.io/badge/Algorithm-Sorting-blue?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyBmaWxsPSJ3aGl0ZSIgcm9sZT0iaW1nIiB2aWV3Qm94PSIwIDAgMjQgMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI%2BPHRpdGxlPlNvcnRpbmc8L3RpdGxlPjxwYXRoIGQ9Ik0zIDVoNFYzaC00em01IDBoNFYzaC00em01IDBoNFYzaC00em01IDBoNFYzaC00ek0zIDEzaDRWOGgtNHptNSAwaDRWOEgtOHptNSAwaDRWOEgtMTN6bTUgMGg0VjhoLTR6TTMgMjFoNFYxNmgtNHptNSAwaDRWMTZoLTh6bTUgMGg0VjE2aC00em01IDBoNFYxNmgtNHoiLz48L3N2Zz4%3D&logoColor=white&labelColor=000000"
         alt="Algorithm Sorting">
  </a>
<a href="https://github.com/jdecorte-be/push-swap/blob/master/Makefile">
    <img src="https://img.shields.io/badge/Build-Makefile-4298B8?logo=gnu-make&logoColor=white&labelColor=000000"
         alt="Build Makefile">
  </a>
</p>

<p align="center">
<a href="https://github.com/jdecorte-be/push-swap/actions">
    <img src="https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white&labelColor=000000"
         alt="CI/CD GitHub Actions">
  </a>
  <a href="https://github.com/jdecorte-be/push-swap">
    <img src="https://img.shields.io/badge/topic-42--school-66D9EF?logo=github&logoColor=white&labelColor=000000"
         alt="push-swap 42-school">
  </a>
  <a href="https://github.com/jdecorte-be/push-swap">
    <img src="https://img.shields.io/badge/topic-algorithm-66D9EF?logo=github&logoColor=white&labelColor=000000"
         alt="push-swap algorithm">
  </a>
  <a href="https://github.com/jdecorte-be/push-swap">
    <img src="https://img.shields.io/badge/topic-c-66D9EF?logo=github&logoColor=white&labelColor=000000"
         alt="push-swap c">
  </a>
  <a href="https://github.com/jdecorte-be/push-swap/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/License-GPL--3.0-AE81FF?labelColor=000000"
         alt="push-swap license">
  </a>
  <a href="https://github.com/jdecorte-be/push-swap/stargazers">
    <img src="https://img.shields.io/github/stars/jdecorte-be/push-swap?logo=star&logoColor=white&labelColor=000000&color=E6DB74"
         alt="push-swap stars">
  </a>
</p>
<p align="center">
  <a href="#pushswap-instructions">push_swap instructions</a> •
  <a href="#compilation">Compilation</a> •
  <a href="#execute">Execute</a> •
  <a href="#tester">Tester</a> •
  <a href="#part-i-preparing-for-solving">Part I: Preparing for solving</a> •
  <a href="#part-ii-from-stack-a-to-stack-b">Part II: From Stack A to Stack B</a> •
  <a href="#part-iii-from-stack-b-to-stack-a">Part III: From Stack B to Stack A</a>
</p>
</header>

The **push_swap** project is a very simple and highly effective algorithm project: data will need to be sorted. You have at your disposal a set of int values, 2 stacks and a set of instructions to manipulate both stacks.

This project contains 2 programs:
- The first, named **checker** which takes integer arguments and reads instructions on the standard output. Once read,checker executes them and displays `OK` if integersare sorted. Otherwise, it will display `KO`.
- The second one called **push_swap** which calculates and displays on the standard output the smallest progam using *push_swap instruction language* that sorts inte-ger arguments received.

## push_swap instructions

- **sa**: *swap a* - swap the first 2 elements at the top of stack a. Do nothing if there is only one or no elements.
- **sb**: *swap b* - swap the first 2 elements at the top of stack b. Do nothing if there is only one or no elements.
- **ss**: sa and sb at the same time.
- **pa**: *push a* - take the first element at the top of b and put it at the top of a. Do nothing if b is empty.
- **pb**: *push b* - take the first element at the top of a and put it at the top of b. Do nothing if a is empty.
- **ra**: *rotate a* - shift up all elements of stack a by 1. The first element becomes the last one.
- **rb**: *rotate b* - shift up all elements of stack b by 1. The first element becomes the last one.
- **rr**: ra and rb at the same time.
- **rra**: *reverse rotate a* - shift down all elements of stack a by 1. The last element becomes the first one.
- **rrb**: *reverse rotate b* - shift down all elements of stack b by 1. The last element becomes the first one.
- **rrr**: rra and rrb at the same time.

## Compilation

Compile checker: `make checker`

Compile push_swap: `make push_swap`

Compile both: `make`

## Execute

checker: `./checker 0 2 3 1` then program's waiting for user input

push_swap: `./push_swap 0 2 3 1`

Note: You can also use debug option `-v` as first parameter to see stacks operations

![alt text](https://github.com/ska42/push_swap/blob/main/img/option_debug_example.png?raw=true)

## Tester

There is a bash script named `script.sh` that generate a array of size n and shuffle then test `push_swap | checker` x times.

```
./script.sh size_array [nb_times]
```

![alt text](https://github.com/ska42/push_swap/blob/main/img/script_example.png?raw=true)

### Part I: Preparing for solving

#### Step 1: Indexation

By the task we know that given numbers cannot contain duplicates. So we can assign index for each number. It will help us in future steps.

The index `0` will be assigned to the smallest number. To the largest number will be assigned the `count of numbers - 1` index.

_Example_
 
Number|Index
-----:|-----:
-2147483648|0
2100|4
220010|6
-1|1
7|2
210815|5
121|3

#### Step 2: Markup

I have two different markup modes:

* `greater than` markup mode
* `by index` markup mode

_At first I use one markup mode in my algorithm, and then I use the second one. Finally, I compare result of their work and display a better result._

During markup, we have to decide which elements we will keep in stack A. Other elements will be moved to the stack B.

We try to keep in stack A as many elements as possible in chosen mode.

At this step we have to find `markup_head` and also make a markup with selected `markup_head` and in given markup mode. `markup_head` is a start element for markup.

To find `markup_head` we make a markup with each element in the stack and then assign as `markup_head` that element which will keep the biggest number of elements in stack A.

If two elements have the same result, as a `markup_head` will be chosen element with smaller index.

#### `greater than` markup mode

Starting from `markup_head` each element must be greater than previous. Elements that are not satisfied this statement will be moved to the stack B.

_Example_

Markup result in `greater than` markup mode with `-2147483648` element as `markup_head`.

Number|Index|Keep in Stack A
-----:|-----:|:-----:
-2147483648|0|`true`
2100|4|`true`
220010|6|`true`
-1|1|`false`
7|2|`false`
210815|5|`false`
121|3|`false`

_Another example_

Markup result in `greater than` markup mode with `-1` element as `markup_head`.

Number|Index|Keep in Stack A
-----:|-----:|:-----:
-2147483648|0|`false`
2100|4|`false`
220010|6|`true`
-1|1|`true`
7|2|`true`
210815|5|`true`
121|3|`false`

#### `by index` markup mode

Starting from `markup_head` each one element must have index greater by 1 than index in previous element. Elements that are not satisfied this statement will be moved to the stack B.

_Example_

Markup result in `by index` markup mode with `-2147483648` element as `markup_head`.

Number|Index|Keep in Stack A
-----:|-----:|:-----:
-2147483648|0|`true`
2100|4|`false`
220010|6|`false`
-1|1|`true`
7|2|`true`
210815|5|`false`
121|3|`true`

### Part II: From Stack A to Stack B

**Pseudocode**

```
WHILE stack A has elements with "false" value in "Keep in Stack A" field
      IF sa (swap a) is needed
            perform sa (swap a) command
            update markup
      ELSE IF head element of stack A has "false" value in "Keep in Stack A" field
            perform pb (push b) command
      ELSE
            perform ra (rotate a) command
```

#### How to check that `sa (swap a)` is needed?

You have to perform `sa (swap a)` and then remake markup. We only have to update markup with chosen at previous steps parameters (as `markup_head`).

Then we have to compare how many elements will be kept in stack A with performed `sa (swap a)` and without it.

If after performing `sa (swap a)` more elements will be kept, it means that there is a reason to do it.

After all we have to unmake `sa (swap a)` and return result of our calculations.

### Part III: From Stack B to Stack A

**Pseudocode**

```
WHILE stack B is not empty
      choose element in stack B for moving to stack A
      move stack A and stack B to prepare them for pa (push a) with chosen element
      perform pa (push a) command
```

### How to choose element in stack B for moving to stack A?

We have to calculate how many commands we need to perform for moving element from stack B to the top of its stack and how many commands we need to perform for moving suitable element from stack A to the top of its stack.

We have to calculate this value for each element in stack B and then choose element with the smallest calculated value and move it to stack A.

### Part IV: Align Stack A

And the last one task is to align stack A. We have to move stack A while the smallest element is not on the top of stack.

### Important

I perform this algorithm two times. At first time I use one markup mode, and then I use another. Finally, I compare result of their work and display a better result.
