# item_modifier-set_enchantments
item_modifierの1項目であるset_enchantmentsのサンプルになります。

詳しくはブログ記事『[【マイクラ】set_enchantmentsでエンチャント付与【item_modifier】](https://natsumake.com/item_modifier-set_enchantments/)』を参考にしてください。

<h3>概要</h3>
アイテムにエンチャントを付与させることができます。

<h3>使い方</h3>

データパック導入後、ワールドに入り```/reload```と入力し実行してください。

タラを倒すことで幸運Ⅲのエンチャントが付与されたダイヤモンドの斧をドロップします。<br>
この幸運Ⅲはset_enchantmentsで付与したものです。

また、以下のコマンドを実行することで、無限Ⅲと効率強化Ⅲのエンチャントを手元のアイテムに付与することが出来ます。<br>
この時、元々付与されている同一のエンチャントはレベルを合算します。

```copy
/item modify entity @s weapon.mainhand sample:set_enchantments
```

その一方で、以下のコマンドで付与させた場合には元々付与されていたエンチャント内容を上書きします。<br>
つまり、レベルの合計などは関係なく、指示したレベルへと変化してしまいます。

※新規に付与されるエンチャントについては、ただ付与されるだけです。<br>
元々付与されており、以下のコマンドで参照しているitem_modifier内に記載されていないエンチャントについては変化が起きません。

```copy
/item modify entity @s weapon.mainhand sample:set_enchantments_replace
```
