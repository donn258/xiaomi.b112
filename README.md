# xiaomi.b112
озвучка для пылесоса xiaomi.vacuum.b112
этот пылесос постороен на очень простом процессоре esp32 что чудовишно не хватает для нормайной работы пылесоса
спецификация у данного пылесоса точно такая же как и у пылесосов ijai
raw команда для установки озвучки, например немецкого:

{"method":"action","params":{"aiid":1,"did":"","in":[{"piid":1,"value":"de_DE"},{"piid":5,"value":"https://cdn.cnbj2.fds.api.mi-img.com/ijai-lite-map.record/audio_v24/german.bin"},{"piid":6,"value":"82b39dbd00f720df75a4687df0de0f1b"}],"siid":14}}

этой командой можно установить озвучку например через:
1) автоматизацию Mihome используя кастомное приложение от vevs
2) с сайта https://vacuum.mindsolo.net/ в разделе "Терминал" вашего пылесоса
3) используя python MiIO

голосовые пакеты у данной модели находятся в формате bin, несжатый wav format: 88.2 kb/s, 11.025 kHz, 8 bits, 1 channel, PCM (Unsigned)
