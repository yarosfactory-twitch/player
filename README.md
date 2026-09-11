# player

OBS Browser Source плеєр для yarosfactory — вбудовує YouTube або SoundCloud трек за параметром у URL.

Хоститься через GitHub Pages, щоб мати справжній https-домен (обхід бага OBS Browser Source з `Referer`-заголовком і error 153 при прямому embed з YouTube).

## Використання в OBS

Додай Browser Source з URL:

**YouTube:**
```
https://<твій-github-юзер>.github.io/player/?v=VIDEO_ID
```

**SoundCloud:**
```
https://<твій-github-юзер>.github.io/player/?sc=https://soundcloud.com/.../track
```

`VIDEO_ID` — це частина після `v=` у звичайному посиланні YouTube (`youtube.com/watch?v=ЦЕ_ID`).

Щоб поміняти трек під час стріму — просто заміни параметр `?v=...` у налаштуваннях джерела в OBS і натисни OK.

## Як увімкнути GitHub Pages для цього репо

1. Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main`, папка `/ (root)`
4. Save — за пару хвилин сторінка стане доступна за адресою вище
