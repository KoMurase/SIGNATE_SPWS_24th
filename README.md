SIGNATE 医学論文の自動仕分けチャレンジ(https://signate.jp/competitions/471) 
に参加した時のリポジトリ

最終的に採用したコードをまとめました．

models にあるモデルの内12個を用いて，出力の確率値をLightGBMの入力として，
スタッキングを行った．
LightGBMは，パラメータ変更を行い，gbdt, dart, rfの三種類別々に学習を行った．

最終的には，gbdt, dart, rfのCV値により重みづけアンサンブルを行い，提出した．
