# Timothy Meehan's new laptop request

I have been using my laptop - a Dell Inc. Latitude 7410 - since I joined. My laptop has never been particularly fast but my working experience has significantly worsened over the last 12 months with the new stack.

It has reached a point where I can barely start the main front-end application, front-office.

- Starting the application and seeing changes in the browser takes a lot of time.
- The IDE (type intellisense, linting, ...) suffers from serious latency.
- I can't start the application and host a VS Code Live Share session
- Having Zoom + the IDE open + the dev application is impossible

My battery life barely **holds no more than 1 hour**, [see screenshot](./battery_life.png)

## Comparison with other laptops

I have asked some of my colleagues who have M1 and M3 macbooks to run some commands to highlight the difference of speed. Below is the result table.

- `dev`: command to start the main application in dev mode
- `tsc`: command to perform type-checking
- `setup`: command to setup the mono-repository (the Nuxt framework goes over the codebase and generates necessary files)

| Command | My Laptop (Latitude 7410) | Macbook M1 2020         | Macbook M3 2023         |
| ------- | ------------------------- | ----------------------- | ----------------------- |
| dev     | 2300ms                    | 800ms **(2.8x faster)** | 679ms **(3.3x faster)** |
| tsc     | 56s                       | 31s (**1.8x faster**)   | 27s (**2x faster**)     |
| setup   | 2mins18                   | 56s (**2.4x faster**)   | 48s (**2.8x faster**)   |

The screenshots are available in the folders

- [my laptop](./my-laptop-benchmark/)
- [macbook m1](./macbook-m1-benchmark/)
- [macbook m3](./macbook-m3-benchmark/)
