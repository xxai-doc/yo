<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

O ti wa ni niyanju lati fi sori ẹrọ nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) akọkọ, ati ki o `direnv allow` lẹhin titẹ awọn liana ( [awọn .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yoo wa ni ṣiṣẹ laifọwọyi lẹhin titẹ awọn liana).

Itumọ ni: Itumọ Kannada si Japanese, Korean, English, English translation si gbogbo awọn ede miiran. Ti o ba fẹ lati ṣe atilẹyin Kannada ati Gẹẹsi nikan, o le kan kọ `zh: en` .

## iwaju-opin koodu

* [iwaju-opin koodu](https://github.com/xxai-art/web)
* [Awọn akopọ ede fun aaye naa lapapọ](https://github.com/xxai-art/web/tree/main/i18n)
* [Awọn akopọ ede fun awọn modulu iwọle](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Oju opo wẹẹbu Multilingual Documentation](https://github.com/xxai-doc)

Ede siseto iwaju-opin jẹ [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , eyiti o ṣafikun diẹ ninu awọn ẹya ti o da lori sintasi kọnputa kofi, wo [./coffee_plus.md](./coffee_plus.md) .

## Internationalization ti awọn aaye ayelujara ati awọn iwe aṣẹ

Kọ lori awọn wọnyi 3 ise agbese

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Suffix naa jẹ `.mdt` , o le lo sintasi ti o jọra si `<+ ./coffee_plus/import.js>` lati tọka si awọn faili ita, ati ṣe ipilẹṣẹ isamisi pẹlu suffix `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Itumọ ti samisi kii yoo tumọ awọn koodu ati awọn ọna asopọ, yoo si kaṣe awọn gbolohun ọrọ ti a tumọ. Tí ìtúmọ̀ náà bá jẹ́ títúnṣe ṣùgbọ́n tí a ko ṣàtúnṣe ọ̀rọ̀ ìpilẹ̀ṣẹ̀, títúnṣe rẹ̀ kò ní tún ìtumọ̀ náà kọ.

* [@ w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Awọn faili ede fun titumọ awọn oju opo wẹẹbu ti ipilẹṣẹ `yaml` .

### Awọn Itọsọna Adaaṣe Itumọ Iwe

Wo ibi ipamọ koodu [xxai-art/doc](https://github.com/xxai-art/doc)

O ti wa ni niyanju lati fi sori ẹrọ nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) akọkọ, ati ki o `direnv allow` lẹhin titẹ awọn liana ( [awọn .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yoo wa ni ṣiṣẹ laifọwọyi lẹhin titẹ awọn liana).

Lati yago fun ipilẹ koodu nla ti a tumọ si awọn ọgọọgọrun awọn ede, Mo ṣẹda ipilẹ koodu lọtọ fun ede kọọkan ati ṣẹda agbari kan lati tọju ipilẹ koodu

Ṣiṣeto iyipada ayika `GITHUB_ACCESS_TOKEN` ati lẹhinna ṣiṣe [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) yoo ṣẹda ibi ipamọ koodu laifọwọyi.

Dajudaju, o tun le fi sii ni ipilẹ koodu kan.

Itọkasi iwe afọwọkọ itumọ [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Awọn koodu iwe afọwọkọ jẹ itumọ bi atẹle:

[bunx](https://bun.sh/docs/cli/bunx) jẹ aropo fun npx, eyiti o yarayara. Nitoribẹẹ, ti o ko ba ti fi sori ẹrọ bun, o le lo `npx` dipo.

`bunx mdt zh` renders `.mdt` ninu iwe ilana zh bi `.md` , wo awọn faili 2 ti o ni asopọ ni isalẹ

* [kofi_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kofi_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` jẹ koodu mojuto fun itumọ (ti o ba ti fi sori ẹrọ `nodejs` nikan, ṣugbọn `bun` ati `direnv` ko fi sii, o tun le ṣiṣe `npx i18n` lati tumọ).

O yoo parse [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , iṣeto ni ti `i18n.yml` ninu iwe yi jẹ bi wọnyi:

```
en:
zh: ja ko en
```

Itumọ ni: Itumọ Kannada si Japanese, Korean, English, English translation si gbogbo awọn ede miiran. Ti o ba fẹ lati ṣe atilẹyin Kannada ati Gẹẹsi nikan, o le kan kọ `zh: en` .

Awọn ti o kẹhin ni [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , eyi ti o jade awọn akoonu laarin awọn akọle akọkọ ati awọn akọkọ atunkọ ti kọọkan ede `README.md` lati se ina kan titẹsi `README.md` . Koodu naa rọrun pupọ, o le wo funrararẹ.

Google API ni a lo fun itumọ ọfẹ. Ti o ko ba le wọle si Google, jọwọ tunto ati ṣeto aṣoju kan, gẹgẹbi:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Iwe afọwọkọ itumọ naa yoo ṣe ipilẹṣẹ kaṣe ti a tumọ ninu itọsọna `.i18n` , jọwọ ṣayẹwo rẹ pẹlu `git status` ki o ṣafikun si ibi ipamọ koodu lati yago fun awọn itumọ ti atunwi.

Jọwọ ṣiṣe `bunx i18n` ni gbogbo igba ti o ba ṣe atunṣe itumọ lati ṣe imudojuiwọn kaṣe naa.

Ti ọrọ atilẹba ati itumọ ba jẹ atunṣe ni akoko kanna, kaṣe naa yoo dapo, nitorina ti o ba fẹ yipada, o le ṣe atunṣe ọkan nikan, lẹhinna ṣiṣe `bunx i18n` lati ṣe imudojuiwọn kaṣe naa.
