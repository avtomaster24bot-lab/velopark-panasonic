# Velopark.kz — Panasonic landing page

Готовый адаптивный одностраничный сайт на чистом HTML/CSS/JS. Никаких сборщиков и платных библиотек не требуется.

## Быстрый запуск на GitHub Pages

1. Распакуйте архив.
2. Загрузите `index.html`, `README.md` и папку `assets` в корень репозитория GitHub.
3. Откройте **Settings → Pages**.
4. В разделе **Build and deployment** выберите **Deploy from a branch**, ветку `main` (или `master`) и папку `/ (root)`, нажмите **Save**.
5. Через несколько минут GitHub Pages покажет адрес опубликованного сайта.

## Telegram

Все основные CTA уже ведут на `https://t.me/GrifRift555`.

## Фотографии и оформление

Все фото на сайте — реальный велосипед (Panasonic BE-EPE63). Оригиналы уменьшены до 1280–1600 px по длинной стороне, JPEG ~82%, без EXIF. Для карточек и галереи используются облегчённые копии из `assets/thumbs/` (640 px), по клику в лайтбоксе открывается полный размер из `assets/`.

Единственное нереальное изображение — `anime-panasonic*.jpg`: аниме-иллюстрация для первого экрана (на сайте подписано «Иллюстрация в стиле аниме»).

Файлы в `assets/`:
- `01-overall-left.jpg`
- `02-overall-right.jpg`
- `03-front.jpg`
- `04-rear.jpg`
- `05-motor.jpg`
- `06-battery.jpg`
- `08-battery-connector.jpg`
- `09-control-panel.jpg`
- `10-control-panel-on.jpg`
- `11-nexus-hub.jpg`
- `12-inter3-marking.jpg`
- `13-shifter-3speed.jpg`
- `15-inter-m-brake.jpg`
- `16-cooling-disc.jpg`
- `18-front-brake.jpg`
- `19-front-brake-detail.jpg`
- `21-front-wheel.jpg`
- `21b-front-wheel.jpg`
- `27-model-plate.jpg`
- `27b-baa-sticker.jpg`
- `27c-registration-sticker.jpg`
- `28-panasonic-frame.jpg`
- `30-panasonic-light.jpg`
- `30b-light-lens.jpg`
- `31-rear-reflector-panasonic.jpg`
- `32-front-reflector-basket.jpg`
- `33-rear-reflector.jpg`
- `34-wheel-lock.jpg`
- `36-handlebar-lock.jpg`
- `37-rack.jpg`
- `37b-rack-top.jpg`
- `42-stand-lock.jpg`
- `42b-stand-lock.jpg`
- `43-bridgestone-saddle.jpg`
- `45-seatpost.jpg`
- `46-grip-left.jpg`
- `46b-grip-right.jpg`
- `48-handlebar-top.jpg`
- `49-stem.jpg`
- `50-controls.jpg`
- `51-tire-tread.jpg`
- `52-tire-irc.jpg`
- `54-tire-bridgestone.jpg`
- `55-front-fender.jpg`
- `56-rear-fender.jpg`
- `57-pedal-crank.jpg`
- `58-chain.jpg`
- `59-basket.jpg`
- `61-city-shot.jpg`
- `anime-panasonic-800.jpg`
- `anime-panasonic-web.jpg`
- `anime-panasonic.jpg`

Чтобы заменить фото — положите новый файл с тем же именем в `assets/` и (желательно) уменьшенную копию 640 px в `assets/thumbs/`.
Чтобы добавить фото в галерею — скопируйте любой блок `<figure class="g-item g-extra">…</figure>` в `index.html` и поменяйте пути, подпись и `data-cap`.

Дизайн: японский / аниме-стиль (шрифты Google Fonts Zen Maru Gothic + Nunito с кириллицей), падающие лепестки сакуры (canvas), лёгкий параллакс, появление блоков при прокрутке, анимированный велосипед-разделитель. Все анимации отключаются, если в системе включено «уменьшение движения».

## Добавить YouTube-видео

В блоке `video-frame` замените заполнители на iframe, изменив `VIDEO_ID` на ID своего ролика:
```html
<iframe
  src="https://www.youtube-nocookie.com/embed/VIDEO_ID"
  title="Видеообзор электровелосипеда Panasonic"
  style="width:100%;height:100%;min-height:260px;border:0;border-radius:18px"
  loading="lazy"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>
```
Если видео только в Telegram или файлом, лучше сначала опубликовать его на YouTube (доступ по ссылке) или прислать мне ссылку — можно будет встроить корректно.

## Что проверить перед публикацией

- Уточнить цену и добавить её, когда она будет окончательно определена.
- Проверить комплектацию именно этого экземпляра: модель мотора, аккумулятор, втулку, тормоза и маркировки.
- «Керамические тормоза», ёмкость батареи и запас хода на сайте не указаны — добавляйте только подтверждённые данные.
- Допустимая нагрузка багажника на сайте не указана — добавьте, если найдёте маркировку.
- Добавить фактические сроки, стоимость доставки и условия бронирования, если они известны.
