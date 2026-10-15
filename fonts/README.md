# The faces the app ships (131)

Every typeface the app shows is in this folder and served with the app from its own origin: the prompter's curated set (`src/faces.ts`, six faces at regular and bold) and the interface's own (Manrope, JetBrains Mono, Barlow Semi Condensed). Nothing is fetched from a third party. The files are the Latin and Latin Extended subsets as Google Fonts serves them in WOFF2, fetched by the author with Rob's word from `fonts.gstatic.com`: on 14 October 2026 the files Google serves to a current browser (the width probe measured these), and later the same day, for the four faces Google serves as one variable file, the STATIC instances it serves to an older browser, one file per weight, since the line model reads each file's own width table (`tools/fontwidths.js`, 0.5.206) and a variable file carries only its default weight's. The interface's Manrope and JetBrains Mono stay variable, their weight range declared in `prompter-app.css`, which declares every file.

Every family is published under the SIL Open Font License, Version 1.1, whose text is `OFL.txt` beside this file. The copyright line of each family, read on 14 October 2026 from the first line of its `OFL.txt` in the google/fonts repository (`https://raw.githubusercontent.com/google/fonts/main/ofl/<family>/OFL.txt`), verbatim:

- Atkinson Hyperlegible: Copyright 2020 Braille Institute of America, Inc.
- Lexend: Copyright 2018 The Lexend Project Authors (https://github.com/googlefonts/lexend), with Reserved Font Name "RevReading Lexend".
- Inter: Copyright 2020 The Inter Project Authors (https://github.com/rsms/inter)
- Noto Sans: Copyright 2022 The Noto Project Authors (https://github.com/notofonts/latin-greek-cyrillic)
- Source Serif 4: Copyright 2014 The Source Serif 4 Project Authors (https://github.com/adobe-fonts/source-serif)
- Barlow Semi Condensed: Copyright 2017 The Barlow Project Authors (https://github.com/jpt/barlow)
- JetBrains Mono: Copyright 2020 The JetBrains Mono Project Authors (https://github.com/JetBrains/JetBrainsMono)
- Manrope: Copyright 2018 The Manrope Project Authors (https://github.com/googlefonts/manrope)

The licence permits bundling and redistribution with software; no face here is modified, and no reserved font name is used for anything.

Adding a face later takes the same road: an open licence, one fetch by the author into this folder with Rob's word, its width factor read by `deliveries/research/face-width-probe-2026-10-12.html` on a real screen, an entry in `src/faces.ts` with the figure, and a build.

| file | family | weight | subset | bytes | SHA256 |
|---|---|---|---|---|---|
| `atkinson-hyperlegible-400-latin-ext.woff2` | Atkinson Hyperlegible | 400 | latin-ext | 9384 | `61eeb0eb8b881a84d069e67be1723f5b353b0b9b866ad8e7ad9dba66cdc4dabd` |
| `atkinson-hyperlegible-400-latin.woff2` | Atkinson Hyperlegible | 400 | latin | 17208 | `d64ba838ef5472bba248620ec4fd8b5aa7cf0db2908e0bb230600caf279ba7bc` |
| `atkinson-hyperlegible-700-latin-ext.woff2` | Atkinson Hyperlegible | 700 | latin-ext | 9372 | `840ced16f975d8abc2594b436d0206649e0c2a7327e36750ff849d3d37c3c02e` |
| `atkinson-hyperlegible-700-latin.woff2` | Atkinson Hyperlegible | 700 | latin | 17524 | `140e2bd25a7315c8a062508391426b0d8c3297400c947b8d847be28f73a199f0` |
| `barlow-semi-condensed-400-latin-ext.woff2` | Barlow Semi Condensed | 400 | latin-ext | 14448 | `a11398bc7ca9c39ba38fcc24d84ddc233a28d751d7e25eb5e27da0d9c8ae1a2d` |
| `barlow-semi-condensed-400-latin.woff2` | Barlow Semi Condensed | 400 | latin | 22300 | `d03a7a5f6b74534c80699289d4f6495fdb09a7596774a4ede79129d2f8bb67b1` |
| `barlow-semi-condensed-500-latin-ext.woff2` | Barlow Semi Condensed | 500 | latin-ext | 14524 | `5e07c7d621bb57be13250d12c8c7ba71b84c6f71ad2080bc2ee9d3dd533b3579` |
| `barlow-semi-condensed-500-latin.woff2` | Barlow Semi Condensed | 500 | latin | 22428 | `0d7513795eaf8fdab7f340144841bd2d9fac7d9303c03aa6b525a2c908e9b371` |
| `barlow-semi-condensed-600-latin-ext.woff2` | Barlow Semi Condensed | 600 | latin-ext | 14848 | `5a58c6c9887c7306399176e96bdeb0c2c3b2935a43f89e25ac4e342b03631843` |
| `barlow-semi-condensed-600-latin.woff2` | Barlow Semi Condensed | 600 | latin | 22984 | `f158417e9207b5362f9b71a2fe779ce5bb836ad972f38445c3163af39d2c998d` |
| `barlow-semi-condensed-700-latin-ext.woff2` | Barlow Semi Condensed | 700 | latin-ext | 15076 | `109b73c772cc798422a6879f32c96ad646cb65f5c211933cb05f60c4fc2ab540` |
| `barlow-semi-condensed-700-latin.woff2` | Barlow Semi Condensed | 700 | latin | 23244 | `fb958c8c20a05552ac8a85d925d96028d52565792650e941a5fe96b6997aa5cb` |
| `inter-400-latin-ext.woff2` | Inter | 400 | latin-ext | 35000 | `6744a7f509ebc6ab220a6cd4ea77e898adf014f03d88dcda5d45d8a9feefb4e9` |
| `inter-400-latin.woff2` | Inter | 400 | latin | 23664 | `8909904ab6c872eb994093482a88a28eca2cd95912d7b6fecd72103b0dc07edc` |
| `inter-700-latin-ext.woff2` | Inter | 700 | latin-ext | 36244 | `143f9504f1377012aa3e39c90c4354ef429cb0494b9ac0e1437f1a81e5412236` |
| `inter-700-latin.woff2` | Inter | 700 | latin | 24356 | `6f56409fd3d64bb85f7d070bce20749db2d66b6d63cec586cc22d1c761be2491` |
| `jetbrains-mono-variable-latin-ext.woff2` | JetBrains Mono | 400, 500 | latin-ext | 11624 | `db5ff4db83e580426280e9337a58dc57d3a83784a1b03ad80914651594441d52` |
| `jetbrains-mono-variable-latin.woff2` | JetBrains Mono | 400, 500 | latin | 31432 | `83c005d49d8a6a50474c73a5a36ac0468076e9c4a29da7bdb14995d80560a5be` |
| `lexend-400-latin-ext.woff2` | Lexend | 400 | latin-ext | 13144 | `b7289189cf6efefd520224a63a24bc02054f8566f33e39ce9d1a448ccd8a40a4` |
| `lexend-400-latin.woff2` | Lexend | 400 | latin | 14476 | `0601e0a909219a542cdd581e3f8f1ff8fb208978cbc9bca1c90df02fd8062bb1` |
| `lexend-700-latin-ext.woff2` | Lexend | 700 | latin-ext | 13708 | `5ae459b6dc29461eab9f02d0ff4395d3842d6bdf280e8224a79ab2667e65ee2f` |
| `lexend-700-latin.woff2` | Lexend | 700 | latin | 14808 | `52dcdaa127bac4a5ea4c39ee17a3f454ceacc18d9f2a45cc453eeab68d378588` |
| `manrope-variable-latin-ext.woff2` | Manrope | 400, 500, 600, 700 | latin-ext | 15120 | `3911b66d9f2e005a4b989223405d0e5032619c668597ba467cc76a23c8fffcfb` |
| `manrope-variable-latin.woff2` | Manrope | 400, 500, 600, 700 | latin | 24836 | `a30ddcd349703aff7464c34bef3fffdff405ee50c113440d7c8693c02d210972` |
| `noto-sans-400-latin-ext.woff2` | Noto Sans | 400 | latin-ext | 55640 | `c8e6bf928ae88c948ebc49dbe1df01ea5505d12408904ea3302309b26487fbca` |
| `noto-sans-400-latin.woff2` | Noto Sans | 400 | latin | 13120 | `09aee8065d25508f23a4c3d92cd777ac869c52d93fd868a88f025d888a7937d6` |
| `noto-sans-700-latin-ext.woff2` | Noto Sans | 700 | latin-ext | 59144 | `c0cd431266a7ed82d6f0dfe281e38a883c28a03eec1fdac308cc2f7c0ea39c3b` |
| `noto-sans-700-latin.woff2` | Noto Sans | 700 | latin | 13464 | `e77bfe1db912f687b0319b60de158cfada67f89c8ee4f8e2bd6020f970accbfb` |
| `source-serif-4-400-latin-ext.woff2` | Source Serif 4 | 400 | latin-ext | 17844 | `78ff74ea29d0cc5594ff9efd5c0a30911691b89e9021e7bcf118b95e285e007f` |
| `source-serif-4-400-latin.woff2` | Source Serif 4 | 400 | latin | 20088 | `02194deb92d3975dd30e11a3824a1f1db32b48c93654e60560cb81ce8e7b5f95` |
| `source-serif-4-700-latin-ext.woff2` | Source Serif 4 | 700 | latin-ext | 18468 | `06e2c39d92b45e61e0988b141fdc61632f77e5e7d793e225ee7eb9e307333308` |
| `source-serif-4-700-latin.woff2` | Source Serif 4 | 700 | latin | 21716 | `7691c51bc286a9014db0048277d2c3f2ad0a90b533dc8adfb16cb22a95390d39` |
