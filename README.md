# opf-on-gpu

## How to run the script?
First, julia v1.9 needs to be installed. We recommend using [juliaup](https://github.com/JuliaLang/juliaup). To benchmark with Ma27Solver, you can additionally install [JuliaHSL](https://www.hsl.rl.ac.uk/hsl2023/index.html). The script assumes that your computer has an NVIDIA GPU.

Once julia is installed, you can instantiate the project to automatically download the dependencies.
```
$ cd path/to/opf-on-gpu
$ julia --project -e 'import Pkg; Pkg.instantiate()`
```
Then, the script can run:
```
$ julia -e 'include("example.jl"); include("example.jl")' 
```
Here, we run it twice just to make sure that compilation time is not affecting the timing results.