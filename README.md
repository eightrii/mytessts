Отключение FSO - это как Hyperthreading (SMT) - зависит от игры. ЭТО НЕ ПРАВИЛО. Необходимо разделить игры Dx12 и Dx11. Игры Dx12 выигрывают от FSO, а Dx11 и некоторые порты Dx12 - нет. Независимо от названия, настройки видео в игре должны быть всегда на Fullscreen для лучшего задержки ввода. Alt-Tabbing в некоторых играх работает медленнее, потому что Windows требуется время для выхода из полноэкранного режима и перехода на рабочий стол (медленный переход на рабочий стол также может быть результатом несоответствия игровых разрешений/частоты обновления и настроек рабочего стола). Это просто "переключение скоростей" Windows, это не является признаком или доказательством того, что игра работает с повышенной задержкой ввода. Причина, по которой alt-tabbing работает быстрее в режимах Borderless или Windowed, заключается в том, что рабочий стол уже буферизован. FSO - это оптимизированный безграничный режим. По сути, вы играете на рабочем столе, а GPU одновременно рендерит и рабочий стол, и игру, поэтому WIndows не нужно "переключаться" при переключении alt-tabbing, рабочий стол уже рендерится вместе со всем, что происходит в фоновом режиме - это вызывает задержку ввода. Вы можете потенциально исправить медленный alt-tab, отключив композицию рабочего стола (я не думаю, что она может быть полностью отключена в Win10 без отключения DWM) или принудительно включив старый режим alt-tabbing. 

Теперь совсем другой разговор о том, что этот Fullscreen Mode не является настоящим Fullscreen, но это наиболее близкий "к металлу", как Microsoft позволяет нам быть без полного отключения DWM. В FSO проще реализовать различные виды оверлеев в виде всплывающих уведомлений или когда вы используете наушники или клавиатуру, чтобы уменьшить громкость или яркость, например. В FSE это все еще возможно, но сложнее реализовать и есть риск сбоя, особенно при Alt-Tabbing на рабочий стол или в программу, а Dx12 скоро станет единственным API, на котором будут создаваться игры, и они не будут использовать FSE, но все равно будут быстрее, чем игры на Dx11. Microsoft медленно внедряет улучшения Dx12, а Nvidia и AMD следуют за ней со своими драйверами. Такие вещи, как Mesh Shading, Variable Rate Shading и Variable Resolution невозможны в Dx11, но они снижают использование процессора и значительно повышают производительность. Вы все еще можете отключить FSO в реестре или отключить DWM для лучшей отзывчивости/производительности.
