# Philosophers

This project is about learning the basics of process threading using mutexes, semaphores and avoiding data races.
The **dining philosophers problem**, formulated in 1965 by Edsger Dijkstra, can be summed up as following:

> - One or more philosophers sit at a round table, and there is a plate of spaghetti in the middle
> - On the table, there are as many forks as there are philosophers
> - The philosophers can either, eat, think or sleep
> - In order to eat, each philosopher needs to use 2 forks
> - When a philosopher has finished eating, they put their forks back on the table and start sleeping
> - The simulation stops when a philosophers dies of starvation.

![philo1](https://github.com/dubmix/42-philosophers/assets/104844198/501f9d4c-42b4-4d9d-9a9a-b2171ffe69c1)

The `number of philosophers`, `time to die`, `time to eat`, `time to sleep` and optional `number of times each philospher must eat` are the arguments
to the program (time in ms).

## Usage

Warning: `Makefile` is configured for `Linux` use only.

> - Compile with `make`
> - Then run with `./philo` and for example `4 800 300 200'. In this case the program runs indefinitely
> - Running with for example `2 401 200 200` will work as well
> - With `2 400 200 200`, a philosopher will die and the simulation stops

Here is how running `./philo 4 800 300 200' looks like in the terminal:

![philo2](https://github.com/dubmix/42-philosophers/assets/104844198/206d89c1-d5c4-4bc5-877f-e7082bdee1a5)

And here is a visualization of what's actually happening:

![philo3](https://github.com/dubmix/42-philosophers/assets/104844198/5dec53d7-8e62-48fa-977c-532de1a7eae7)

## Restrictions

This project is written in C and 42 norm compliant:

> - All variables have to be declared and aligned at the top of each function
> - One function cannot have more than 25 lines
> - It is considering cheating to use functions that are forbidden in the subject
