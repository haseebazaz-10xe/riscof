##Downloading the repo
```
git clone https://gitlab.com/incoresemi/riscof.git
git checkout experimental

```
Before proceeding further please ensure that riscv-toolchain and spike simulator is installed.

##Install dependencies
```
pip install -r requirements.txt

```
##Running the simulation

Macro definition file - riscof/framework/env
test file path - suite/I-ADD-01.S

command-
```
python -m riscof.main -bm model_from_yaml -bf Examples/template_env.yaml -dm model_from_yaml -ispec Examples/rv32i_isa.yaml -pspec Examples/rv32i_platform.yaml -eyaml Examples/template_env.yaml --verbose debug

```

Results shall be generated in work/