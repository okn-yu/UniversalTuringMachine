# UniversalTuringMachine
- 万能チューリングマシンの実装です
- チューリングマシンはCOMETのエミュレータとして動作を想定しています
- 入力データはCASLで符号化されていることを想定しています
- Haskellで実装しています

## 実装方針
- 最初はチューリングマシンのテープと遷移関数は脇においてHaskell単体でCOMETのエミュレータを作成する
- エミュレータ完成後にチューリングマシンに移植する

## テープ
- チューリングマシンには2つのテープが存在することを想定しています。
- 1本目のテープにはメモリやレジスタが利用する領域を想定しています。
- 2本目のテープには処理対象となるCOMETのプログラムが記載されていることを想定しています。
