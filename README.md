# Notepad++ for Hongkonger

This repo is created for **Hong Kong Cantonese** localization for Notepad++.

All translations are done by human base on:

- **All about Hong Kong:** Not Macau Cantonese, not Guangzhou Cantonese, but Hong Kong Cantonese! This localization contains some words only used by Hongkongers.
- **How we communicate in daily life:** Hong Kong culture is unique mixture of Chinese, British and Western culture in general. We speak Cantonese with some English together. Especially for some technology terms, I would like to retain some English words.
- **A little bit Taiwan:** We'd got lots of benefit from Taiwan software and books - Eten (倚天中文系統), PC Home, BBS, and more. Remember the old days? I would adapt some terms from Taiwanese Mandarin, if they are not available in Hong Kong.

The localization is done based on Notepad++ v7.8.9 Stand With Hong Kong Edition. Welcome issues and pull requests.

:heart: Notepad++. :heart: Hong Kong. :heart: Hongkongers.


## Install and Test

### In Windows UI

For common users to install and test it in Notepad++:

1. You can download this repo directly.
1. Unzip the downloaded file, properly called `<notepad-plus-plus-localization-hong-kong-master>`.
1. Copy and replace the XML file `<nativeLang.xml>` in your user settings with the file `<hongKongCantonese.xml>` in this repo.

	|           | Source                    | Target             |
	| --------- | ------                    | ------             |
	| File name | `<hongKongCantonese.xml>` | `<nativeLang.xml>` |
	| Directory | Root of this repo         | `<%USERPROFILE%\AppData\Roaming\Notepad++\>` |

1. Restart Notepad++ to apply the change.

To revert the localization: On Notepad++ menu, click 設定 (Settings) ▶︎ 偏好設定 (Preference) ▶︎ choose an option in 本地化 (Localization).


### Via Command Prompt

For better experience, you can use Command Prompt to help a little bit:

```cmd
:: Clone from my repo or yours
git clone https://github.com/Edditoria/notepad-plus-plus-localization-hong-kong.git
cd notepad-plus-plus-localization-hong-kong

:: Get submodule
git submodule init
git submodule update

:: Inject (Copy) to Notepad++
.\tools\inject.cmd .\hongKongCantonese.xml
```

Every time you make some changes, you can use the above "inject" command to update. Restart Notepad++ to take effect.

---

The above information is written for Notepad++ developers and international users. From now on, I would write in Hong Kong Cantonese.


## 本地化嘅宗旨

Notepad++ 轉介面語言嘅講法係叫 localization 而唔係 translation，所謂本地化，唔係一味轉晒啲字做中文就算，而係要真實咁反映我哋嘅文化，要貼近日常生活。所以，我係以呢啲方針嚟寫嘅：

- 我哋香港人平日點講嘢，個 repo 就用番咩字眼，如果要求書面語，用番台灣正體中文版咪得囉，駛乜搞咁多嘢。
- 盡量尊重番英文版嘅精神同埋用字，例如 file vs document，就跟番寫「檔案」同「文件」。
- 如果某個正字本身好少見人寫，甚至乎冇乜人識睇，跟返約定俗成就好，我哋做嘢以人為本，唔好太追求文字本源。
- 香港人日常寫信都已經中英夾雜，假如某個字已經係用英文為主，就直接用番英文，例如「嘥屎」，與其譯做「大細」唔湯唔水，不如直接寫「size」。
- 香港人早年受台灣電腦書薰陶，介面用慣英文同台灣正體中文，有啲 case 諗唔到點譯做港語嘅，跟番台式中文咪算囉。
- 輕微嘅俗語 okay 但係粗口就免喇，始終 Notepad++ 嘅用家對象係全年齡向。

每一句我都會重複想像情境，例如响 office：

- 嗰句嘢**兜口兜面點樣講出嚟**，
- **聽嗰位人兄聽唔聽得明**。

總之，譯嘢要符合生活情景，文化傳承要貼地丶本土，唔求優雅唔怕庸俗。


## 呢個 Repo 嘅 Status

本來都係龜速咁慢慢寫，但係 Notepad++ Stand With Hong Kong Edition 出咗兩版，又適逢 Github 嘅 Hacktoberfest 2020，我就 push 個 repo 出嚟，大家一齊玩玩丶一齊 fix。

- 呢個 repo 名應該叫「香港廣東話」丶「香港粵語」定係叫「香港語」，注意要能夠配合番譯做英文要睇得明，仲有跟 Notepad++ 選擇語言嘅一致性。 **（希望盡早決定）**
- Typo丶錯別字丶文法。
- 整體嚟講啲字詞丶語法等嘅用字，有冇一致性嘅問題。
- 實際畫面上有冇 overflow 嘅問題，搞到啲字顯示唔到响個 mon 到，歡迎搵搵 XML comment 咗 `<-- #todo reproduce -->` 嘅 line。冇顯示問題嘅話，大可以開 PR 摌走個 comment；有顯示問題，就開個 issue。
- 用字上，正字丶異體字同埋約定俗成點樣拿捏（例如「d」vs「啲」），仲有 Windows 字型顯示（例如「𠹺」丶「𡁵」），需要大家討論。


## 社群貢獻指引（簡潔版）

- 麻煩跟番上面「宗旨」嗰段嘅精神。
- PR (Pull Requests) 盡量細分，容易 review，例如成個 repo 所有 files 出現一個錯字/詞語，一口氣一個 PR，而另一個錯字/詞語，另開一個 PR。
- 如果唔肯定，歡迎開個 issue 傾傾。
- 只會 accept 對 localization 內容有幫助嘅 PR。
- No spam. 鐵定嚴格執行。
- 麻煩參考 `<.editorconfig>`，跟番 EOL 字元丶tab/space，盡量啦唔該。 🙏


## Todo

- [ ] `<hongKongCantonese.xml>` 裏面仲有好多錯處，歡迎大家參與。
- [ ] 改善 `<tools\>` 啲 scripts 嘅體驗。
- [ ] 一啲 Github 建議嘅社群文件，例如 `<CONTRIBUTING.md>` 。
