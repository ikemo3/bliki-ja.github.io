---
title: ネットワーク型データモデル
tags: [database]
---

http://martinfowler.com/bliki/NetworkDataModel.html

ネットワーク型データモデルとは、データをレコード形式にし、レコード間をポインタでリンクさせたものである。そのため、ネットワーク型データモデルにクエリを発行するには、あるレコードから出発し、ポインタで参照してまわるという形になる。

ネットワーク型モデルのデータベースは少し前に人気が落ち、[[RelationalDataModel]]にとって代わられた。しかし、まったく使われていないというわけではない。実は、メモリ内のデータというのは、基本的には、ネットワーク型データモデルなのである。現在主流である言語のほとんどが、レコード型とポインタを定義する機能を持っている。

オブジェクトモデルをネットワーク型データモデルだと考えることもできる。というのも、オブジェクトもデータ構造をもっており、ポインタでリンクされているからだ。決定的な違いは、オブジェクトはデータと振る舞いを一緒にしている点だろう。そのため、実際に使うときには、両者に差異を感じるかもしれない。しかし、多くのオブジェクトモデル（[[貧血症のドメインモデル|AnemicDomainModel]]など）にはこれといった振る舞いは含まれておらず、単にネットワーク型データモデルになっているようだけれども。