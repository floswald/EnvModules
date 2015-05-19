

# Environment Module Files

this repo contains some environment module files that I have found useful.

## Usage

On a system with [Environment Modules](http://en.wikipedia.org/wiki/Environment_Modules_%28software%29), it is quite easy to create your own module. you can just modify any of the given examples contained in this repo. As an example, suppose you installed `gcc 4.9.0` into your home directory at `~/local/gcc4.9` and want to create a modulefile for it, such that you can write

```bash
module load compilers/gcc4.9
```

and that takes care of setting all environment variables. here's how:

```bash
git clone https://github.com/floswald/EnvModules
module use-append ~/git/EnvModules/modulefiles
module avail   # this should include your custom modules now
               # of course you will have to change the paths
```


