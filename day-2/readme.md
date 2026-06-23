## Day 2 Automated DFT with PWTK

### Session Goals

1. Create a Quantum ESPRESSO input file  
2. Use the Quantum ESPRESSO input generator  
3. Run your first Quantum ESPRESSO calculation  
4. Introduction to PWTK  
5. Hands on comparison of PWX and PWTK with Xcrysden  
6. Parameter optimisation using PWTK  
7. Using ASE, Materials Project, and QE input generators  

---

## Alias and Environment Setup

### Creating aliases in Linux

Aliases help you run long commands using short names.
* * *
Examples  
- `xi` for `xcrysden --pwi`  
- `xo` for `xcrysden --pwo`  
- `xsf` for `xcrysden --xsf`  

### Safe way to add aliases and paths

```bash
echo "alias xi='xcrysden --pwi'" >> ~/.bashrc
echo "alias xo='xcrysden --pwo'" >> ~/.bashrc
echo "alias xsf='xcrysden --xsf'" >> ~/.bashrc
echo 'export PATH="$PATH:/home/qe/espresso"' >> ~/.bashrc
````

Reload the configuration

```bash
bash ( in current terminal or open new terminal)
```

### Important note

Be careful while editing the `~/.bashrc` file. Incorrect changes can affect your shell environment.

To edit manually

```bash
vim ~/.bashrc
```

Add aliases or paths, then save and exit using

```
:wq
```

This setup allows you to run scripts from the espresso directory from anywhere in the terminal.
