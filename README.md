# KlausHome 封面库

家庭影院（Emby / DrivEmby 系播放器）分类封面图，16:9 WebP，与 KH 图标库相互独立。本仓库内含三套可切换主题，播放器选对应 JSON 直链填入。

## 目录结构

```
emby-covers/
├── covers.json          # 主题一：暗调电影感封面清单
├── covers-cyber.json    # 主题二：霓虹赛博风封面清单
├── covers-poster.json   # 主题三：影视海报风封面清单
├── README.md
├── covers/              # 主题一 14 张 16:9 WebP（电影感）
├── covers-cyber/        # 主题二 14 张 16:9 WebP（霓虹赛博）
└── covers-poster/       # 主题三 14 张 16:9 WebP（影视海报）
```

## 播放器怎么填

三套主题各一条 JSON raw 直链，按当前想用的风格粘贴到「添加封面库 / 背景图库 → URL」：

**主题一 · 暗调电影感（默认）**

```
https://raw.githubusercontent.com/cle7er/emby-covers/main/covers.json
```

**主题二 · 霓虹赛博风**

```
https://raw.githubusercontent.com/cle7er/emby-covers/main/covers-cyber.json
```

**主题三 · 影视海报风**

```
https://raw.githubusercontent.com/cle7er/emby-covers/main/covers-poster.json
```

## 分类与匹配键

JSON 里 `name` 是匹配键，封面按媒体库名称匹配，每个分类除中文名外另附拼音/英文别名兜底。三套主题均为 14 个分类。

| 封面 | 中文名 | 别名 | 电影感 | 赛博风 | 海报风 |
| --- | --- | --- | --- | --- | --- |
| 01_华语电影.webp | 华语电影 | chinese-movie, huayu-movie | ✓ | ✓ | ✓ |
| 02_外语电影.webp | 外语电影 | foreign-movie, waiyu-movie | ✓ | ✓ | ✓ |
| 03_动画电影.webp | 动画电影 | animation-movie, donghua-movie | ✓ | ✓ | ✓ |
| 04_纪录片.webp | 纪录片 | documentary, jilupian | ✓ | ✓ | ✓ |
| 05_儿童.webp | 儿童 | kids, children, ertong | ✓ | ✓ | ✓ |
| 06_国产剧.webp | 国产剧 | chinese-tv, guochanju | ✓ | ✓ | ✓ |
| 07_欧美剧.webp | 欧美剧 | western-tv, oumeiju | ✓ | ✓ | ✓ |
| 08_日番.webp | 日番 | anime-jp, rifan | ✓ | ✓ | ✓ |
| 09_国漫.webp | 国漫 | anime-cn, guoman | ✓ | ✓ | ✓ |
| 10_日韩剧.webp | 日韩剧 | kr-jp-tv, rihanju | ✓ | ✓ | ✓ |
| 11_音乐.webp | 音乐 | music, yinyue | ✓ | ✓ | ✓ |
| 12_未分类.webp | 未分类 | unassigned, weifenlei | ✓ | ✓ | ✓ |
| 13_综艺.webp | 综艺 | variety, zongyi | ✓ | ✓ | ✓ |
| 14_原盘电影.webp | 原盘电影 | yuanpan, original-movie, remux | ✓ | ✓ | ✓ |

## 备注

- 图标库（KH 徽记）在另一个独立仓库 `kh-icons`，与本封面库分开维护、两条独立链接。
- 三套封面同库不同目录；想换风格只需在播放器里把 JSON 直链换成另一套，图片互不覆盖。
- raw 链接依赖 GitHub 域名访问；私有仓库不能直接用 raw 直链。
