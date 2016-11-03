# Pockeが1バン好きなこと



---

# だれこれ

---



# <img style="width: 30%; border-radius: 50%" alt="ほにゃー" src="pocke.svg">


## Masataka Kuwabara (a.k.a. pocke)

- Actcat Inc.
- The Open University of Japan
- Cookpad Summer Internship 2016


---


# 近況

---

## インターン行ってました

- エイチーム
  - 優勝した
- mixi
  - ホットチョコミントおいしかった



---


## ありたそ被害者の会に入会しました

<img src="./aritaso.png" alt="">


---


# 1バン好きなこと
<!-- -attr- data-background="#ED5358" -->

---

## なんだろう…
<!-- -attr- data-background="#ED5358" -->

---

 ### .｡oO(好きなことは多く呟いているのでは…)
<!-- -attr- data-background="#ED5358" -->

---


# しらべてみた
<!-- -attr- data-background="#ED5358" -->

---

<!-- -attr- data-background="#ED5358" -->

1. http://twilog.org/ から過去ツイート一覧のcsvをダウンロード
1. シェル芸
1. 多く呟いている単語を抽出

---

<!-- -attr- data-background="#ED5358" -->

## こんなかんじ

```sh
$ < p_ck_161101.csv | 
  ruby -rcsv -e '
  CSV.parse($<){|row|
    puts row[2].gsub(/\@[a-zA-Z0-9_]+/, "").gsub(%r!https?://\S+!, "")
  }' | 
  head -5000 | docker run -i docker-mecab-neologd:latest | 
  grep '名詞' | cut -f 1 | sort | grep -v '^.$' |
  ruby -e '
  c = 1; p = nil;
  while gets
    if $_.chomp==p then c+=1 else puts "#{c} #{p}"; c=1; p=$_.chomp end
  end' |
  sort -nr | head -30
```

Thanks! https://github.com/nownabe/docker-mecab-neologd


---


<!-- -attr- data-background="#ED5358" -->

## けっか

```
117 感じ
115 自分
103 NowPlaying
101 最近
92 RuboCop
91 人間
86 Ruby
75 好き
71 今日
70 奥華子
69 RT
66 便利
59 dentoolt
56 最高
55 PR
50 問題
49 時間
48 必要
48 ーー
47 Rails
45 会社
44 気分
41 気持ち
39 開発
38 GitHub
38 git
37 英語
37 体調
37 一切
35 明日
35 PC
34 Slack
32 実行
30 仕事
29 お金
28 名前
28 SideCI
27 完全
26 設定
26 学生
```

---


<!-- -attr- data-background="#ED5358" -->

## 結論

---


<!-- -attr- data-background="#ED5358" -->

- NowPlaying 多め
- RuboCop / Ruby 好き
- 奥華子最高!!!


---

<!-- -attr- data-background="#ed538e" -->

# 閑話休題

---

<!-- -attr- data-background="#ed538e" -->

# 実は今までの話は前置き


---

<!-- -attr- data-background="#ed538e" -->

## 本題: <br>今私が一番好きで<br>話したいこと！！

---


<!-- -attr- data-background="#ed538e" -->

# 本

---


## 本を買うのが好き

<!-- -attr- data-background="#ed538e" -->
<img src="./book_tw.png" alt="">


---

<!-- -attr- data-background="#ed538e" -->

# 本棚の様子


---

<!-- -attr- data-background="#ed538e" -->


---
