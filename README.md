# graphviz-events
Uma aplicação do graphviz e do pré-compilador do cpp para visualização vetorial de eventos históricos

## overview

- graph1.gv (input data)
- graph.svg (output data, svg vectorial image, generated by dot/graphviz command)
- /w40 (images of country flags)

## system tools

sudo apt install imagemagick
sudo apt install gcc
sudo apt install graphviz

## script data 

nano/vim graph1.gv

## compiling data (graph1.gv) with gcc/graphviz to vetorial image format (graph.svg)

dot -Tsvg <(cpp graph1.gv) > graph.svg

## if needed, you can compose dual flags using convert command (imagemagick)

convert pt.png br.png +append ptbr.png
