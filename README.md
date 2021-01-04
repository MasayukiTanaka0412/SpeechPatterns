# ソフトウェア・エンジニアのためのスピーチパターン
  
![表紙](images/kaigi_man.png)
  
2021年1月
  
著：田中　真幸
  
Copyright (C) 2021  TANAKA Masayuki  
  
[コンテンツはこちら](ビジネスにおける再利用のためのスピーチパターン.md)
  
## 執筆環境
  
- Visual Studio Code
- [vscode-pandoc](https://marketplace.visualstudio.com/items?itemName=DougFinke.vscode-pandoc)
- [pandoc](https://github.com/jgm/pandoc/releases/tag/2.11.3.2)
- [TeXインストーラ 3](https://www.ms.u-tokyo.ac.jp/~abenori/soft/abtexinst.html)
  
## 設定
  
- vscode-pandoc
    -Pandoc:Pdf Opt String
        - -V documentclass=ltjsreport --pdf-engine=lualatex
  
## ビルド
  
- PDF
    - vscode-pandocで、生成
- EPUB
    - pandoc -f markdown -t epub3 ビジネスにおける再利用のためのスピーチパターン.md title.txt -o ビジネスにおける再利用のためのスピーチパターン.epub --css stylesheet.css --toc --toc-depth=2 --epub-cover-image=cover.jpg