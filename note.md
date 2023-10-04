## For pcb:

### gEDA pcb editor

> prefered option

gEDA editor, has builtin gcode export.

```sh
sudo apt-get install pcb
```

Export as gcode, uncheck all box (predrill, drill-mill, advanced-gcode)

Then use script to fix variable, see zicBox repo


### Kicad pcb editor

> alternative option

The PCB was created with [kicad](https://www.kicad.org/). 

```sh
sudo apt-get install kicad
```

#### Export as SVG

- Select only `F.Cu`
- Set print mode to `Black and white`
- Set SVG Page Size to `Board area only`

> Might want to optimize the svg: `npx svgo encoder-F_Cu.svg -o encoder-F_Cu.optimized.svg`

#### SVG to Gcode

To convert SVG to Gcode, use https://cam.openbuilds.com/

