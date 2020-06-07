# Dyalog APL′ ("Prime")

"Prime" is intended as a rather minimal modification of [Dyalog APL](https://www.dyalog.com/), but going back and correcting original design mistakes. This mostly regards being primary-axis oriented, but also applies to making the original operators consistent and making `⎕IO←0` forced. The goal is to make APL more appealing to the modern audience. That is, to bring APL into its prime.

Requires Dyalog APL version 17.1 or higher.

### How to use

#### Initialisation

Replacing `ns` with your target namespace (e.g. `#`), do

```
]import ns path/prime
```

#### Running code

Now you have three options:

1. Use the extensions directly with the glyph names.
1. Use `ns.prime.FIX` as a drop in for `⎕FIX`.
1. Use `ns.prime.Repl ''` to start a (limited) self-contained session where the glyphs work. Enter `→` to exit.
1. Use `ns.prime.Repl ref` to start a (limited) session in the namespace `ref`. Enter `→` to exit. 

### Content

| Name                                              | Glyph  | Extension                                                    |
| ------------------------------------------------- | :----: | ------------------------------------------------------------ |
|[BackSlashBar](BackSlashBar.aplf)|`⍀`|only expand first|
|[CircleBackSlash](CircleBackSlash.aplf)|`⍉`|monadic rotates axes|
|[CircleBar](CircleBar.aplf)|`⊖`|disabled|
|[CircleStile](CircleStile.aplf)|`⌽`|first axis|
|[Comma](Comma.aplf)|`,`|first axis|
|[CommaBar](CommaBar.aplf)|`⍪`|increase rank/join|
|[DelStile](DelStile.aplf)|`⍒`|but dyadic sort-by|
|[DeltaStile](DeltaStile.aplf)|`⍋`|but dyadic sort-by|
|[DownArrow](DownArrow.aplf)|`↓`|enclose major cells|
|[DownShoe](DownShoe.aplf)|`∪`|on major cells|
|[DownTack](DownTack.aplf)|`⊤`|transposed and extend scalar|
|[Epsilon](Epsilon.aplf)|`∊`|on major cells|
|[Iota](Iota.aplf)|`⍳`|noticing 1-element vector|
|[IotaUnderbar](IotaUnderbar.aplf)|`⍸`|`⎕IO←0` for monadic but `⎕IO←1` for dyadic|
|[LeftShoe](LeftShoe.aplf)|`⊂`|just `⎕IO`|
|[LeftShoeUnderbar](LeftShoeUnderbar.aplf)|`⊆`|on major cells|
|[Plus](Plus.aplf)|`+`|purely numeric|
|[QuadDivide](QuadDivide.aplf)|`⌹`|high rank|
|[Query](Query.aplf)|`?`|high rank|
|[RightShoe](RightShoe.aplf)|`⊃`|just `⎕IO`|
|[SlashBar](SlashBar.aplf)|`⌿`|only replicate first|
|[Squad](Squad.aplf)|`⌷`|but sane|
|[Tilde](Tilde.aplf)|`~`|on major cells|
|[UpShoe](UpShoe.aplf)|`∩`|on major cells|
|[UpTack](UpTack.aplf)|`⊥`|transposed|
|[\_BackSlash](_BackSlash.aplo)|`\`|scan first and outer product|
|[\_Diaeresis](_Diaeresis.aplo)|`¨`|handling empty arrays with failing prototype|
|[\_JotDiaeresis\_](_JotDiaeresis_.aplo)|`⍤`|but handling empties|
|[\_Slash](_Slash.aplo)|`/`|only reduce first|
