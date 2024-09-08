---
layout: post
title: Komentáře na BoBlogu
subtitle: Přehled různých řešení a je to vůbec potřeba?
readtime: true
gh-repo: mbobcik/BoBlog
gh-badge: [follow]
tags: [komentáře]
---

Ukrutná aktivita na BoBlogu, ale hlavně moje zvědavost mě donutili porozhlédnout se po řešení komentářů k článkům.
Člověk by si řekl "kde je problém? Sekci komentářů má nejeden článek na internetu, a pod zprávama je to hotový zlatý důl národní inteligence!"
A já bych odpověděl, že komentáře samy o sobě problémové tolik nejsou, pokud na ně nemáme žádné požadavky.
Těch ale pár mám, jak funkčních, tak nefunkčních (to jest výrazivo softwarového návrhu).
Priorita je celková cena řešení. 
Z BoBlogu žádný příjem nemám a celkově ho mám spíš jako polo-hobby.
Tím pádem do něj nechci vrážet víc, než by bylo nezbytně nutné.
Počáteční investice i provozní náklady by se měli rovnat nule. 

Dalším kritériem je omezení odesílání jakýchkoliv dat cizím společnostem. 
Obsah komentářů, informace o webu a uživatelích by měli zůstat co nejblíže webu. 
Už tohle, ve spojení s prvním požadavkem, docela drasticky omezuje výběr možností.
Mimo jiné i často používané Facebook Comments.

V neposlední řadě je zde spíš omezení.
A to že BoBlog je staticky generovaný [Jekyll](https://jekyllrb.com/) web.
Jak moc je tohle omezení důležité nevím, ale určitě je na to potřeba myslet při výběru.

Jo, ještě mě napadá: jakékoliv reklamy třetích stran jsou velké \[nou-nou\].
Beztak tady zase takový provoz nemám, aby to případnému poskytovateli zaplatilo náklady.
Pokud už sem ale někdo zavítá, tak vsadím boty, že má buď zapnutou nějakou formu blokování reklamy,
nebo na ni vůbec neklikne.

# Možnosti
Zvyk ze školy velí si nejdříve udělat rešerši dostupných řešení.
V konfiguračním souboru Jekyll témy už jich pár má přípravu.
Ze zajímavosti jsem ještě přidal Webmentions, což je taky taková forma komentářů.
Ty ale implementovat nebudu, je to moc práce a nepřijde mi to tak užitečné :)

## Disqus
[Disqus](https://disqus.com/) je relativně profesionální platforma, která prej umožňuje monetizaci na internetu bez cookies. Nabízí real-time funkcionalitu jako hlasování o jednotlivých komentářích (upvoty a downwoty na Redditu), vlákna odpovědí a podobné moderní vymoženosti. Jako plus určitě beru možnost přidání obrázků a videí do obsahu komentáře. Další výhodou je téměž automatická moderace obsahu a filtry spamu. Na současném internetu je mnoho darmošlapů, kteří rádi škodí všemu hezkému.

Kromě jiného je Disqus sice zadarmo, ale s reklamami. Což je proti mým požadavkům. Za 12$ nebo 272 Korun Českých bych se sice mohl reklam zbavit, ale to už je ukrutně velká částka za malou featuru na ještě menším webu. 

Celkově mi Disqus přijde jako "s kanonem na vrabce". Má příliš mnoho fukncí, které malé weby těžko využijí. Ten můj určitě ne.

## CommentBox

## Staticman

## Utterances

## Giscus

## Mastodon posty

## Webmetions

