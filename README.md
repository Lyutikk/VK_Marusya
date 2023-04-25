[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=Voice+assistant+Marusya)](https://git.io/typing-svg)

<h1 align="center">Решение команды GrowAi на хакатоне СКФО Цифровой прорыв: <i>"Маруся не отвечает на реплики из телевизора"</i></h1>

  <p align="center"><img src="https://grow-ai-marusya-vk-digital.hf.space/media/d5c5f03764cfe8f85490c4edca900b35975b1bd5f4971f4e117e81ce.jpeg" width="800" height="600"></p>
  <h2>Краткое описание кейса</h2>
  <p>Голосовые помощники становятся неотъемлемой частью нашей жизни — они помогают не только нам, но и пользователям разного возраста. Например, одной 
    из ключевых аудиторий для голосового помощника от VK — Маруси являются дети — они общаются с ней как с другом, учатся через нее и получают полезную информацию. 
    Зачастую детская коммуникация с детскими технологиями специфична.
  </p>
  <h2>Проблематика</h2>
  <p>В некоторых случаях вместо фразы пользователя, Маруся может услышать фразу из телевизора, который работает фоном, и ответить на неё, что не очень нравится 
    пользователям. К тому же большинство ответов на произвольный набор слов будут нерелевантны.
  </p>
  <h2>Решение</h2>
  <p>Решение кейса представляет собой модель, которая будет понимать, что фраза не от пользователя, а от телевизора. Тогда Маруся смогла бы не отвечать на такие фразы.</p>
  <h2>Данные</h2>
  <p>Данные содержат в себе 3 столбца. В первом столбце содержится фраза для которой необходимо сделать предсказание, является ли она обращением к Марусе или нет. 
    Второй столбец содержит в себе контекст диалога с Марусей. Данный диалог предшествовал целевой фразе(предсказание делается именно для одной конкретной фразы из 
    первого столбца). Если диалог заполнен пропусками, то диалога с Марусей до нее не было, либо человек молчал. Третий столбец содержит в себе целевую переменную. 
    1 – если фраза не обращена к Марусе, 0 – если фраза предназначалась ей. 
  </p>
  <h2>Формат датасета:</h2>
  <p><b>текст фразы пользователя  \t контекст общения с Марусей \t метка </b></p>
  <p>‘\t’ - разделитель</p>
  <h2>Exploratory Data Analysis</h2>
  <p><b>Общий shape</b> - 28 901 записей, из которых:</p>
  <p> - 22 788 релевантных (присвоен класс 0)</p>
  <p> - 6 113 нерелевантных (присвоен класс 1)</p>
  <p></p>
