# ruby\_parts

## CL::RFind

### Example

```
git clone https://github.com/LightningDAISY/ruby\_parts.git
bin/rfind -p ~/Documents/ -e txt [Pp]assword
```

### Concept

mdfindの自分用です。
実行オプション等は -h を参照してください。


## CL::Parser

### Example

```
bin/example.rb -a -b B1 -c C1 -c C2 -c C3 "this is a pen"
```

result

```
{:a=>[], :b=>["B1"], :c=>["C1", "C2", "C3"]}
["this is a pen"]
```

### Concept

標準のパーサが趣旨と違うので作りました。

1. 例外になりません
2. 順不同です
3. 長いオプション名もそのまま解釈します
4. 戻り値が型揺れしません
5. コマンドもオプションも複数渡せます
6. クオートで括ったコマンドをそのまま返します。
7. つまり "this is a pen" をそのまま返します。
8. usageは各自で用意してください


