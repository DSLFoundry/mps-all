# Binary distribution
A list of binary distributions can be found on [releases wiki page](https://github.com/slisson/mps-all/wiki).

# Build instructions
Get a copy of the repository:
```bash
git clone https://github.com/slisson/mps-all.git
cd mps-all
git submodule update --init --recursive
```

Build the plugins with ant (windows instructions)
```bash
mkdir mps-math\solutions\de.itemis.mps.editor.math.runtime\source_gen
mkdir mps-math\languages\de.itemis.mps.editor.math\source_gen
mkdir mps-tables\languages\de.slisson.mps.tables\runtime\source_gen
mkdir mps-tables\languages\de.slisson.mps.tables\source_gen
ant -Dmps.home="<MPS folder>"
```

The produced plugin pack can be found in `build\artifacts\mps-sl-all\mps-sl-all.zip`.

Install this pack by extracting `mps-sl-all.zip` to `<MPS directory>/plugins`.