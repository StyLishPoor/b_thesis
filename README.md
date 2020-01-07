Sample of tex files for b-thesis.

## 卒論添削時の注意

nelio さんが書いてくれた注意事項を転記しておく．

- 参考文献のフォーマット
   - Nov. なのか November なのか
   - H. Watanabe なのか Hiroki Watanabe なのか
   - Proc. なのか Proceeding なのか，Trans. なのか Transaction なのか
- 主語述語の対応が取れているのか
- 「〜とか」を使う場合は「XXとか，YYとか」のように呼応させるとか
- 「〜を行う」は使わない（設定を行う → 設定する にする）
   - 最後に 行う で検索を書けてチェック
- 図のキャプションの末尾にはピリオドを打つ．
- 英語の省略形の書き方の統一
   1. Application Function Chaining (AFC)  私はコッチ派
   1. AFC (Application Function Chaining)
- トラフィック or トラヒック（トラフィックのほうが一般的だって聞いた）
- キャプションの位置は「表の上」，「図の下」
- 1つ or 一つ or ひとつ の統一
- 参照漏れの確認（? で検索をかける）

## How to see diff in github.com

`[github.comのリモートリポジトリのURL]/compare/[比較元のcommit, tag, branch]...[比較先のcommit, tag, branch]` にアクセスすることで，github.com上で比較できます．
第n稿を書き上げたタイミングでcommitにtagを打っておくと比較しやすいでしょう．

## Filename

ファイル名にprefixをつけることで，github.com上でのdiff表示の順序制御をしています．
基本的に `xx-hogehoge.tex` と順番をつけていますが，章構成の変更などで間に章を追加したくなることがあると思います．
例えば，関連研究（ `02-related_work.tex` ）と設計（ `03-design.tex` ）の間にアプローチの章を入れる場合は， `02_1-approach.tex` のように， `_` で間に値を挟むと順序が保存されるので，そうしてください．
`04-design.tex` のようにリネームしてしまうと，リネーム前後でdiffを取れなくなるので，リネームするのはオススメしません．
