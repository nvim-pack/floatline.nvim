# Benchmark for some statusline
   Many lua statuslines say they are fast. Is it true?

   It benchmark a redraw time.
   Every time you type a key or run vim.cmd the statusline need to draw again a few time.
   On insert mode with lsp server it redraw statusline a lot more than 20 time with 1 keystroke.

   Benchmark result is updated by github CI bot. It run 10.000 time

##Result
``` log
Update by bot:
Sun Oct 24 03:13:04 UTC 2021

Time airline: 6.107585084
Text:
 NORMAL  lua/benchmark.lua                                       1% ㏑:1/55☰℅:1 


Time lightline: 0.520466807
Text:
 NORMAL  benchmark.lua                       unix | utf-8 | no ft    1%    1:1  


Time galaxyline: 2.700283449
Text:
▊   1.4k  benchmark.lua  1 : 1   Top                               benchmark▊


Time windline: 0.450042608
Text:
 NORMAL  benchmark.lua 1.38k                             l/n   1:1    1% 


Time lualine: 0.550884661
Text:
 NORMAL  benchmark.lua                               utf-8 | unix    1%    1:1  


Time feline: 1.525168078
Text:
▊     benchmark.lua  1.38k    1:0                                   Top ▁▁


Time staline: 0.597114804
Text:
                       benchmark.lua                    [1/55] :1 並1%  


Time neoline: 0.733868762
Text:
NORMAL                                                    🧊   utf-8  1:1


Time mini: 0.349340881
Text:
 N  lua/benchmark.lua                                                1|55│ 1|40 


Time empty: 0.060946394
Text:
 ~/work/floatline.nvim/floatline.nvim/lua/benchmark.lua  utf-8       C:1 L:1 Top

```
