# Тыквовин — карты ведущего

Схемы для стола, не картинки. Имена как в [приключении](adventure.md). Север сверху. Цифра на схеме = метка; у метки одна фраза «что здесь». Бой — [статблоки](adversaries.md), варка — [brewing.md](brewing.md). Промпты для картинок — в конце файла. Отдельные SVG (открыть в браузере): [городок](maps/ryzhiy-log.svg) · [двор](maps/usadba-dvor.svg) · [этаж](maps/dom-etazh.svg) · [подвал](maps/dom-podval.svg) · [теплица](maps/teplitsa.svg).

---

## 1. Рыжий Лог (весь городок сверху)

Телега приезжает с юга по колее через поля. Гостиница стоит у этой дороги: окна смотрят на путь к Урсагу; рядом стойло — телегу и лошадь прячут туда, не оставляют на улице. Площадь — коротко вглубь городка. Усадьба на северной окраине, не у площади.

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 1020" width="100%" role="img" aria-label="Рыжий Лог сверху">
  <defs>
    <pattern id="fld" width="28" height="14" patternUnits="userSpaceOnUse">
      <rect width="28" height="14" fill="#2a3a2e"/>
      <path d="M0 10 Q14 5 28 10" stroke="#3d4f42" stroke-width="1.1" fill="none"/>
    </pattern>
    <radialGradient id="glow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#f0d080" stop-opacity="0.85"/>
      <stop offset="100%" stop-color="#f0d080" stop-opacity="0"/>
    </radialGradient>
  </defs>
  <rect width="900" height="1020" fill="#1c2430"/>
  <rect x="16" y="48" width="868" height="956" fill="url(#fld)" rx="8"/>

  <!-- road N-S -->
  <rect x="292" y="160" width="58" height="820" fill="#6e5a45"/>
  <rect x="318" y="160" width="6" height="820" fill="#8a7358" opacity="0.55"/>
  <!-- ruts on south stretch -->
  <path d="M310 790 C308 850 312 920 309 990" stroke="#4a3b2c" stroke-width="2.2" fill="none"/>
  <path d="M338 790 C340 850 336 920 341 990" stroke="#4a3b2c" stroke-width="2.2" fill="none"/>

  <!-- estate -->
  <rect x="214" y="66" width="286" height="96" rx="6" fill="#e8d4a8" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="214" y="66" width="286" height="22" rx="6" fill="#8b6b3e"/>
  <text x="357" y="122" text-anchor="middle" fill="#1a140c" font-size="15" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Усадьба Урсага</text>
  <text x="357" y="142" text-anchor="middle" fill="#5a4630" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">окраина</text>
  <g><circle cx="236" cy="88" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="236" y="88" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">8</text></g>

  <text x="390" y="230" text-anchor="start" fill="#dcc9a0" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">несколько минут пешком</text>

  <!-- quiet houses (east of the inn stable) -->
  <rect x="710" y="700" width="48" height="36" rx="3" fill="#cbb896" stroke="#3d2e1a" stroke-width="1.4"/>
  <rect x="764" y="700" width="42" height="32" rx="3" fill="#cbb896" stroke="#3d2e1a" stroke-width="1.4"/>
  <rect x="710" y="748" width="40" height="30" rx="3" fill="#cbb896" stroke="#3d2e1a" stroke-width="1.4"/>
  <text x="748" y="806" text-anchor="middle" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">дома, тихо</text>

  <!-- square -->
  <rect x="368" y="468" width="226" height="148" rx="5" fill="#4a4034" stroke="#d4893a" stroke-width="1.8"/>
  <!-- tents -->
  <polygon points="392,560 412,500 432,560" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <polygon points="450,566 474,508 498,566" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <polygon points="520,558 540,506 560,558" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <!-- scrawny pumpkins -->
  <circle cx="410" cy="580" r="6" fill="#b56a28"/>
  <circle cx="430" cy="586" r="5" fill="#c47a3a"/>
  <circle cx="500" cy="582" r="5" fill="#b56a28"/>
  <circle cx="548" cy="578" r="6" fill="#c47a3a"/>
  <text x="481" y="612" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Площадь · Стамеска</text>
  <g><circle cx="384" cy="486" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="384" y="486" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">3</text></g>

  <!-- shops -->
  <rect x="616" y="486" width="154" height="112" rx="4" fill="#c4a06a" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="616" y="486" width="77" height="112" fill="none" stroke="#3d2e1a" stroke-width="1.4"/>
  <!-- closed doors X -->
  <rect x="640" y="540" width="28" height="40" fill="#6e5a45" stroke="#3d2e1a"/>
  <path d="M640 540 L668 580 M668 540 L640 580" stroke="#1a140c" stroke-width="2"/>
  <rect x="718" y="540" width="28" height="40" fill="#6e5a45" stroke="#3d2e1a"/>
  <path d="M718 540 L746 580 M746 540 L718 580" stroke="#1a140c" stroke-width="2"/>
  <text x="654" y="518" text-anchor="middle" fill="#1a140c" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Гвоздь</text>
  <text x="732" y="518" text-anchor="middle" fill="#1a140c" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Шпулька</text>
  <text x="693" y="582" text-anchor="middle" fill="#1a140c" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">закрыты</text>
  <g><circle cx="632" cy="504" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="632" y="504" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">5</text></g>

  <!-- short street -->
  <rect x="456" y="616" width="44" height="72" fill="#6e5a45"/>
  <text x="548" y="656" text-anchor="start" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">коротко</text>

  <!-- inn -->
  <rect x="356" y="688" width="220" height="122" rx="5" fill="#e8d4a8" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="356" y="688" width="220" height="24" rx="5" fill="#8b6b3e"/>
  <!-- windows face the road (west) -->
  <rect x="360" y="728" width="12" height="22" rx="1" fill="#f0d080" stroke="#3d2e1a"/>
  <rect x="360" y="756" width="12" height="22" rx="1" fill="#f0d080" stroke="#3d2e1a"/>
  <rect x="360" y="784" width="12" height="18" rx="1" fill="#f0d080" stroke="#3d2e1a"/>
  <text x="466" y="748" text-anchor="middle" fill="#1a140c" font-size="15" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">«Свежая Пышка»</text>
  <text x="466" y="770" text-anchor="middle" fill="#5a4630" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">гостиница</text>
  <g><circle cx="376" cy="710" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="376" y="710" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">2</text></g>
  <text x="328" y="768" text-anchor="end" fill="#f0d080" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">окна</text>

  <!-- inn stable: wagon + horse, not on the street -->
  <rect x="582" y="698" width="112" height="108" rx="4" fill="#c4a06a" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="582" y="698" width="112" height="18" fill="#8b6b3e"/>
  <rect x="598" y="730" width="52" height="28" rx="2" fill="#8b6b3e" stroke="#3d2e1a"/>
  <circle cx="608" cy="762" r="6" fill="#3d2e1a"/>
  <circle cx="640" cy="762" r="6" fill="#3d2e1a"/>
  <ellipse cx="666" cy="748" rx="16" ry="10" fill="#6e5a45" stroke="#3d2e1a"/>
  <text x="638" y="790" text-anchor="middle" fill="#1a140c" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">стойло</text>
  <g><circle cx="598" cy="716" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="598" y="716" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">9</text></g>

  <!-- road label -->
  <text x="248" y="740" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">дорога</text>
  <text x="248" y="756" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">к Урсагу</text>
  <g><circle cx="248" cy="718" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="248" y="718" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">4</text></g>

  <!-- town lights -->
  <circle cx="321" cy="840" r="42" fill="url(#glow)"/>
  <circle cx="338" cy="836" r="7" fill="#f0d080"/>
  <text x="250" y="850" text-anchor="middle" fill="#f0d080" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">огни</text>
  <g><circle cx="250" cy="828" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="250" y="828" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">6</text></g>

  <!-- shadow crossing the road into fields -->
  <ellipse cx="430" cy="930" rx="110" ry="28" fill="#0d1016" opacity="0.55" transform="rotate(-12 430 930)"/>
  <path d="M530 918 L610 900" stroke="#0d1016" stroke-width="6" stroke-linecap="round" opacity="0.4"/>
  <text x="640" y="896" text-anchor="middle" fill="#c8b8a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">тень → поля</text>
  <g><circle cx="540" cy="908" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="540" y="908" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">7</text></g>

  <!-- cart track label -->
  <text x="200" y="980" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">колея</text>
  <g><circle cx="200" cy="958" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="200" y="958" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">1</text></g>
  <text x="80" y="200" text-anchor="middle" fill="#9bb394" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">ПОЛЯ</text>
  <text x="820" y="200" text-anchor="middle" fill="#9bb394" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">ПОЛЯ</text>
  <text x="80" y="980" text-anchor="middle" fill="#9bb394" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">ПОЛЯ</text>
  <text x="820" y="980" text-anchor="middle" fill="#9bb394" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">ПОЛЯ</text>

  <text x="450" y="36" text-anchor="middle" fill="#f3ead4" font-size="18" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Рыжий Лог</text>
  <g transform="translate(820,40)">
  <polygon points="0,-18 6.5,9 -6.5,9" fill="#f3ead4"/>
  <rect x="-1.6" y="8" width="3.2" height="8" fill="#f3ead4"/>
  <text x="0" y="32" text-anchor="middle" fill="#f3ead4" font-size="12" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">СЕВЕР</text>
</g>
</svg>

**Легенда**

1. Колея через поля — телега гильдии, погоня, волки хотят мясо.
2. Гостиница «Свежая Пышка» — сдают мясо Марте; из окон видна дорога к Урсагу.
3. Площадь фестиваля — палатка Стамески; сюда вываливают мешок.
4. Дорога к Урсагу — проходит рядом с «Пышкой»; ближе к ночи по ней ковыляют тыквы.
5. Лавки Гвоздя и Шпульки — кузнец и портниха закрыты, груз утром.
6. Огни Рыжего Лога — конец погони, свора отстаёт.
7. Тень Бублика — огромная тень пересекла дорогу и ушла в поля.
8. Усадьба Урсага Корнеплода — окраина, не у площади; дальше карта 2.
9. Стойло у «Пышки» — телега с ящиком и лошадь сюда, не на улицу.

**Пешком.** Гостиница–площадь коротко (одна улица). Гостиница–усадьба несколько минут; на варке пробежка за ящиком — раунд туда, раунд обратно.

---

## 2. Усадьба Урсага Корнеплода

Калитка на юг, в Рыжий Лог. Теплица севернее дома, не впритык: группа сначала упирается в дом. План теплицы — раздел 3: зоны DH (Melee / Very Close / Close), не сетка; джек занимает её целиком, мелкие у стекла и снаружи.

### А. Двор сверху

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 780 900" width="100%" role="img" aria-label="Усадьба Урсага, двор сверху">
  <defs>
    <pattern id="ydfld" width="28" height="14" patternUnits="userSpaceOnUse">
      <rect width="28" height="14" fill="#2a3a2e"/>
      <path d="M0 10 Q14 5 28 10" stroke="#3d4f42" stroke-width="1.1" fill="none"/>
    </pattern>
  </defs>
  <rect width="780" height="900" fill="#1c2430"/>
  <rect x="10" y="50" width="760" height="840" fill="url(#ydfld)" rx="6"/>

  <!-- fence -->
  <rect x="70" y="70" width="640" height="760" fill="#243028" stroke="#5c4a32" stroke-width="10" rx="4"/>
  <rect x="80" y="80" width="620" height="740" fill="#2c382c" stroke="none"/>

  <!-- greenhouse, north, not flush with house -->
  <rect x="250" y="100" width="280" height="130" rx="4" fill="#2f4a42" stroke="#8fbc8f" stroke-width="2.4"/>
  <!-- glass panes -->
  <path d="M250 143 H530 M250 186 H530 M343 100 V230 M437 100 V230" stroke="#8fbc8f" stroke-width="1" opacity="0.7"/>
  <ellipse cx="390" cy="168" rx="52" ry="40" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.6"/>
  <text x="390" y="172" text-anchor="middle" fill="#1a140c" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">джек</text>
  <text x="390" y="248" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Теплица · чуть дальше дома</text>
  <g><circle cx="268" cy="118" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="268" y="118" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">8</text></g>

  <!-- gap / lantern sightline -->
  <path d="M390 230 L390 300" stroke="#f0d080" stroke-width="2" stroke-dasharray="6 5"/>
  <text x="510" y="276" text-anchor="start" fill="#f0d080" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">видна с фонарём</text>

  <!-- house -->
  <rect x="200" y="300" width="380" height="170" rx="4" fill="#e8d4a8" stroke="#3d2e1a" stroke-width="2.2"/>
  <rect x="200" y="300" width="380" height="28" fill="#8b6b3e"/>
  <text x="390" y="390" text-anchor="middle" fill="#1a140c" font-size="16" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Дом Урсага</text>
  <text x="390" y="412" text-anchor="middle" fill="#5a4630" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">записи — план Б</text>
  <g><circle cx="222" cy="328" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="222" y="328" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">5</text></g>

  <!-- cellar window on north wall, facing greenhouse -->
  <rect x="350" y="296" width="80" height="14" rx="2" fill="#1c2430" stroke="#f0d080" stroke-width="1.6"/>
  <text x="510" y="308" text-anchor="start" fill="#f0d080" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">окошко</text>
  <g><circle cx="330" cy="304" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="330" y="304" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">6</text></g>

  <!-- porch south -->
  <rect x="300" y="470" width="180" height="44" rx="2" fill="#c4a06a" stroke="#3d2e1a" stroke-width="1.8"/>
  <text x="390" y="498" text-anchor="middle" fill="#1a140c" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">крыльцо</text>
  <!-- burrow -->
  <ellipse cx="390" cy="526" rx="28" ry="12" fill="#1a140c"/>
  <text x="430" y="548" text-anchor="start" fill="#f3ead4" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">нора</text>
  <circle cx="390" cy="526" r="3" fill="#d4893a"/>

  <!-- barrels by wall -->
  <ellipse cx="230" cy="488" rx="16" ry="12" fill="#8b6b3e" stroke="#3d2e1a"/>
  <ellipse cx="258" cy="488" rx="16" ry="12" fill="#8b6b3e" stroke="#3d2e1a"/>
  <text x="244" y="512" text-anchor="middle" fill="#dcc9a0" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">бочки</text>

  <!-- well -->
  <circle cx="620" cy="430" r="28" fill="#4a6d7c" stroke="#f3ead4" stroke-width="2"/>
  <circle cx="620" cy="430" r="12" fill="#1c2430"/>
  <text x="620" y="478" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">колодец</text>
  <g><circle cx="588" cy="412" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="588" y="412" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">7</text></g>

  <!-- barn west, door ajar to yard -->
  <rect x="100" y="560" width="150" height="130" rx="3" fill="#c4a06a" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="100" y="560" width="150" height="20" fill="#8b6b3e"/>
  <!-- ajar door swinging into yard -->
  <rect x="248" y="600" width="36" height="70" rx="2" fill="#8b6b3e" stroke="#3d2e1a" transform="rotate(-28 248 670)"/>
  <text x="175" y="630" text-anchor="middle" fill="#1a140c" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Сарай</text>
  <text x="175" y="650" text-anchor="middle" fill="#5a4630" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">мешки</text>
  <g><circle cx="118" cy="580" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="118" y="580" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">4</text></g>
  <text x="300" y="640" text-anchor="start" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">дверь приоткрыта</text>

  <!-- cart at gates -->
  <rect x="340" y="720" width="100" height="46" rx="4" fill="#8b6b3e" stroke="#3d2e1a" stroke-width="1.6"/>
  <circle cx="358" cy="770" r="10" fill="#3d2e1a"/>
  <circle cx="422" cy="770" r="10" fill="#3d2e1a"/>
  <text x="390" y="748" text-anchor="middle" fill="#f3ead4" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">телега</text>
  <g><circle cx="330" cy="732" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="330" y="732" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">2</text></g>

  <!-- gate south -->
  <rect x="330" y="820" width="120" height="18" fill="#6e5a45"/>
  <rect x="338" y="812" width="14" height="34" fill="#5c4a32"/>
  <rect x="428" y="812" width="14" height="34" fill="#5c4a32"/>
  <text x="390" y="862" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">калитка → город</text>
  <g><circle cx="318" cy="830" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="318" y="830" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">1</text></g>

  <!-- hole in west fence -->
  <path d="M70 620 Q58 650 70 680" fill="#2a3a2e" stroke="#1a140c" stroke-width="3"/>
  <ellipse cx="64" cy="650" rx="18" ry="22" fill="#1c2430"/>
  <text x="48" y="710" text-anchor="start" fill="#f3ead4" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">дыра</text>
  <text x="48" y="726" text-anchor="start" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">→ поля</text>
  <g><circle cx="48" cy="648" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="48" y="648" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">3</text></g>

  <text x="390" y="36" text-anchor="middle" fill="#f3ead4" font-size="18" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Усадьба Урсага · двор</text>
  <g transform="translate(720,40)">
  <polygon points="0,-18 6.5,9 -6.5,9" fill="#f3ead4"/>
  <rect x="-1.6" y="8" width="3.2" height="8" fill="#f3ead4"/>
  <text x="0" y="32" text-anchor="middle" fill="#f3ead4" font-size="12" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">СЕВЕР</text>
</g>
</svg>

**Легенда**

1. Калитка — вход со стороны города.
2. Телега у ворот — ящик гильдии снимают здесь.
3. Дыра в заборе — Бублик прогрыз и ушёл в поля.
4. Сарай — дверь приоткрыта; мешки дёргаются; купорос не у входа.
5. Дом и крыльцо — вход; нора Бублика под крыльцом.
6. Подвальное окошко — уровень земли, виден угол теплицы; тыквы уходят сюда.
7. Колодец — вода для варки; Бублик крутится здесь.
8. Теплица — чуть дальше дома; джек внутри, кожура подрагивает. Бой — план 3.

### Б. Дом внутри

Первый этаж. Юг — крыльцо во двор. Север — зад дома, к теплице.

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 780 500" width="100%" role="img" aria-label="Дом Урсага, первый этаж">
  <rect width="780" height="500" fill="#1c2430"/>
  <text x="390" y="32" text-anchor="middle" fill="#f3ead4" font-size="18" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Дом · первый этаж</text>
  <text x="390" y="52" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">север — зад дома, к теплице</text>
  <g transform="translate(720,36)">
  <polygon points="0,-18 6.5,9 -6.5,9" fill="#f3ead4"/>
  <rect x="-1.6" y="8" width="3.2" height="8" fill="#f3ead4"/>
  <text x="0" y="32" text-anchor="middle" fill="#f3ead4" font-size="12" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">СЕВЕР</text>
</g>

  <!-- outer walls -->
  <rect x="90" y="80" width="600" height="300" rx="3" fill="#3d3428" stroke="#c4a06a" stroke-width="4"/>

  <!-- cabinet -->
  <rect x="104" y="94" width="278" height="168" fill="#e8d4a8" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="124" y="130" width="90" height="70" rx="3" fill="#c4a06a" stroke="#3d2e1a"/>
  <text x="243" y="168" text-anchor="middle" fill="#1a140c" font-size="16" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Кабинет</text>
  <text x="243" y="190" text-anchor="middle" fill="#5a4630" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">записи Урсага</text>
  <g><circle cx="126" cy="114" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="126" y="114" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">2</text></g>

  <!-- pantry -->
  <rect x="398" y="94" width="278" height="168" fill="#e8d4a8" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="420" y="124" width="24" height="44" rx="2" fill="#8b6b3e" stroke="#3d2e1a"/>
  <rect x="450" y="124" width="24" height="44" rx="2" fill="#8b6b3e" stroke="#3d2e1a"/>
  <rect x="480" y="124" width="24" height="44" rx="2" fill="#8b6b3e" stroke="#3d2e1a"/>
  <circle cx="620" cy="150" r="14" fill="#d4893a" stroke="#3d2e1a"/>
  <text x="537" y="200" text-anchor="middle" fill="#1a140c" font-size="16" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Кладовая</text>
  <text x="537" y="222" text-anchor="middle" fill="#5a4630" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">семечки · тыковка</text>
  <g><circle cx="420" cy="114" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="420" y="114" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">3</text></g>

  <!-- hall -->
  <rect x="104" y="276" width="572" height="90" fill="#d4c09a" stroke="#3d2e1a" stroke-width="2"/>
  <text x="300" y="328" text-anchor="middle" fill="#1a140c" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">холл</text>
  <!-- stairs down -->
  <rect x="430" y="290" width="70" height="62" fill="#8b6b3e" stroke="#3d2e1a"/>
  <path d="M437 300 H493 M437 312 H493 M437 324 H493 M437 336 H493 M437 348 H493" stroke="#e8d4a8" stroke-width="2"/>
  <text x="548" y="328" text-anchor="start" fill="#1a140c" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">в подвал</text>
  <g><circle cx="444" cy="304" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="444" y="304" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">4</text></g>

  <!-- porch -->
  <rect x="280" y="392" width="220" height="58" rx="2" fill="#c4a06a" stroke="#3d2e1a" stroke-width="2"/>
  <text x="390" y="426" text-anchor="middle" fill="#1a140c" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">крыльцо · юг, во двор</text>
  <g><circle cx="300" cy="412" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="300" y="412" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">1</text></g>
  <ellipse cx="390" cy="466" rx="32" ry="12" fill="#0d1016"/>
  <text x="430" y="488" text-anchor="start" fill="#f3ead4" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">нора</text>
</svg>

Подвал под домом. Окошко в северной стене (на угол теплицы). Лестница — в холл.

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 780 480" width="100%" role="img" aria-label="Дом Урсага, подвал">
  <rect width="780" height="480" fill="#1c2430"/>
  <text x="390" y="32" text-anchor="middle" fill="#f3ead4" font-size="18" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Дом · подвал</text>
  <text x="390" y="52" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">окошко на север — угол теплицы</text>
  <g transform="translate(720,36)">
  <polygon points="0,-18 6.5,9 -6.5,9" fill="#f3ead4"/>
  <rect x="-1.6" y="8" width="3.2" height="8" fill="#f3ead4"/>
  <text x="0" y="32" text-anchor="middle" fill="#f3ead4" font-size="12" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">СЕВЕР</text>
</g>

  <rect x="90" y="80" width="600" height="300" rx="3" fill="#2a241c" stroke="#8b6b3e" stroke-width="4"/>

  <!-- window north -->
  <rect x="340" y="76" width="100" height="16" rx="2" fill="#4a7a6a" stroke="#f0d080" stroke-width="1.8"/>
  <text x="510" y="90" text-anchor="start" fill="#f0d080" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">окошко → теплица</text>

  <!-- shelf west -->
  <rect x="114" y="140" width="120" height="160" rx="3" fill="#c4a06a" stroke="#3d2e1a" stroke-width="1.8"/>
  <path d="M122 180 H226 M122 220 H226 M122 260 H226" stroke="#3d2e1a" stroke-width="2"/>
  <rect x="130" y="148" width="18" height="26" fill="#6e5a45"/>
  <rect x="154" y="148" width="18" height="26" fill="#4a6d7c"/>
  <rect x="178" y="148" width="18" height="26" fill="#6e5a45"/>
  <text x="174" y="320" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">полка</text>
  <g><circle cx="132" cy="158" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="132" y="158" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">8</text></g>

  <!-- cauldron center -->
  <ellipse cx="360" cy="220" rx="48" ry="28" fill="#3d3a38" stroke="#f0d080" stroke-width="2"/>
  <ellipse cx="360" cy="208" rx="32" ry="12" fill="#d4893a" opacity="0.85"/>
  <rect x="348" y="248" width="24" height="18" fill="#5c4a32"/>
  <text x="360" y="286" text-anchor="middle" fill="#f3ead4" font-size="14" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">котёл</text>
  <g><circle cx="318" cy="188" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="318" y="188" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">5</text></g>

  <!-- press east of cauldron -->
  <rect x="430" y="170" width="90" height="80" rx="3" fill="#8b6b3e" stroke="#3d2e1a" stroke-width="1.8"/>
  <rect x="448" y="150" width="54" height="28" fill="#c4a06a" stroke="#3d2e1a"/>
  <text x="475" y="286" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">пресс</text>
  <g><circle cx="448" cy="188" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="448" y="188" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">6</text></g>

  <!-- post -->
  <circle cx="600" cy="210" r="16" fill="#c4a06a" stroke="#3d2e1a" stroke-width="2"/>
  <circle cx="600" cy="210" r="6" fill="#3d2e1a"/>
  <path d="M600 226 L600 268" stroke="#c4a06a" stroke-width="6"/>
  <ellipse cx="600" cy="248" rx="20" ry="12" fill="#d4893a" opacity="0.7"/>
  <text x="600" y="300" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">столб</text>
  <g><circle cx="572" cy="188" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="572" y="188" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">7</text></g>

  <!-- crate / barrel -->
  <rect x="250" y="200" width="40" height="32" fill="#8b6b3e" stroke="#3d2e1a"/>
  <ellipse cx="430" cy="330" rx="22" ry="14" fill="#8b6b3e" stroke="#3d2e1a"/>
  <text x="250" y="250" text-anchor="start" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">ящик</text>
  <text x="430" y="356" text-anchor="middle" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">бочка</text>

  <!-- stairs south, matching hall -->
  <rect x="340" y="340" width="100" height="28" fill="#8b6b3e" stroke="#3d2e1a"/>
  <path d="M348 348 H432 M348 356 H432 M348 364 H432" stroke="#e8d4a8" stroke-width="2"/>
  <text x="390" y="400" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">лестница вверх · сквозняк из норы</text>
</svg>

**Легенда**

1. Крыльцо — вход с юга, во двор; под ним нора.
2. Кабинет — записи Урсага.
3. Кладовая — семечки «Бублику» и забытая тыковка на полке.
4. Лестница — из холла в подвал.
5. Котёл и очаг — Урсаг варит; конец варки — треск стекла в теплице.
6. Пресс — основа зелья; сюда катят бочку со двора.
7. Столб — живая тыква в мешке для калибровки.
8. Полка запасов — старые гербициды, пол гонки.

---

## 3. Теплица (финальный бой)

Севернее дома, не впритык. Сетка 5 ft не нужна: зоны считай **от джека**. Вся теплица до стекла — Close; кольцо вокруг него — Very Close (пасть и плеть); корни — Melee. Дверь с юга, к дому: вход сразу в Close. Отдельный файл: [teplitsa.svg](maps/teplitsa.svg).

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 780 760" width="100%" role="img" aria-label="Теплица Урсага, зоны DH">
  <defs>
    <pattern id="tpsoil" width="22" height="22" patternUnits="userSpaceOnUse">
      <rect width="22" height="22" fill="#2c382c"/>
      <circle cx="6" cy="8" r="1.2" fill="#3d4f42"/>
      <circle cx="16" cy="15" r="1.1" fill="#3d4f42"/>
    </pattern>
  </defs>
  <rect width="780" height="760" fill="#1c2430"/>
  <text x="390" y="32" text-anchor="middle" fill="#f3ead4" font-size="18" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Теплица · джек</text>
  <text x="390" y="52" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">зоны DH от джека · сетки нет</text>
  <g transform="translate(720,36)">
    <polygon points="0,-18 6.5,9 -6.5,9" fill="#f3ead4"/>
    <rect x="-1.6" y="8" width="3.2" height="8" fill="#f3ead4"/>
    <text x="0" y="32" text-anchor="middle" fill="#f3ead4" font-size="12" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">СЕВЕР</text>
  </g>

  <!-- yard around glass -->
  <rect x="24" y="68" width="732" height="560" rx="8" fill="url(#tpsoil)"/>

  <!-- greenhouse frame + glass floor -->
  <rect x="90" y="96" width="600" height="420" rx="4" fill="#2f4a42" stroke="#8fbc8f" stroke-width="7"/>
  <!-- glass sash: architecture, not a 3x3 tactical grid -->
  <path d="M165 96 V516 M240 96 V516 M315 96 V516 M465 96 V516 M540 96 V516 M615 96 V516" stroke="#8fbc8f" stroke-width="1.1" opacity="0.45"/>
  <path d="M90 168 H690 M90 438 H690" stroke="#8fbc8f" stroke-width="1.1" opacity="0.45"/>
  <!-- ridge -->
  <path d="M390 96 V516" stroke="#f0d080" stroke-width="1.6" stroke-dasharray="5 7" opacity="0.55"/>
  <text x="404" y="118" text-anchor="start" fill="#f0d080" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">конёк</text>

  <!-- Close = whole house to the glass -->
  <rect x="100" y="106" width="580" height="400" rx="2" fill="none" stroke="#9bb394" stroke-width="1.8" stroke-dasharray="8 6" opacity="0.7"/>
  <text x="118" y="128" text-anchor="start" fill="#9bb394" font-size="12" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Close</text>

  <!-- Very Close ring around Jack (pour / whip) -->
  <ellipse cx="390" cy="292" rx="168" ry="132" fill="#f0d080" fill-opacity="0.07" stroke="#f0d080" stroke-width="2" stroke-dasharray="7 5"/>
  <text x="390" y="168" text-anchor="middle" fill="#f0d080" font-size="12" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Very Close · пасть / плеть</text>

  <!-- Melee on the root body -->
  <ellipse cx="390" cy="304" rx="92" ry="78" fill="#d4893a" fill-opacity="0.10" stroke="#d4893a" stroke-width="2" stroke-dasharray="4 4"/>
  <text x="390" y="392" text-anchor="middle" fill="#d4893a" font-size="11" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Melee · корни</text>

  <!-- beds west -->
  <rect x="118" y="186" width="78" height="118" rx="3" fill="#5c4a32" stroke="#3d2e1a" stroke-width="1.6"/>
  <rect x="128" y="198" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="158" y="214" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="136" y="246" width="24" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="118" y="368" width="78" height="100" rx="3" fill="#5c4a32" stroke="#3d2e1a" stroke-width="1.6"/>
  <rect x="130" y="384" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="158" y="412" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <!-- beds east -->
  <rect x="584" y="186" width="78" height="118" rx="3" fill="#5c4a32" stroke="#3d2e1a" stroke-width="1.6"/>
  <rect x="596" y="198" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="622" y="226" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="584" y="368" width="78" height="100" rx="3" fill="#5c4a32" stroke="#3d2e1a" stroke-width="1.6"/>
  <rect x="598" y="384" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <rect x="624" y="416" width="22" height="14" rx="2" fill="#6a7a4a"/>
  <text x="157" y="354" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">грядки</text>
  <text x="623" y="354" text-anchor="middle" fill="#dcc9a0" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">грядки</text>
  <g><circle cx="132" cy="200" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="132" y="200" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">3</text></g>

  <!-- Jack: pumpkin head, root body, whip — top-down -->
  <!-- legs -->
  <ellipse cx="352" cy="348" rx="28" ry="18" fill="#4a3a28" stroke="#3d2e1a" stroke-width="1.4"/>
  <ellipse cx="428" cy="350" rx="30" ry="18" fill="#4a3a28" stroke="#3d2e1a" stroke-width="1.4"/>
  <path d="M340 348 C320 370 328 392 348 404" stroke="#5c4a32" stroke-width="7" fill="none" stroke-linecap="round"/>
  <path d="M442 350 C460 372 454 396 436 408" stroke="#5c4a32" stroke-width="7" fill="none" stroke-linecap="round"/>
  <!-- torso of roots -->
  <ellipse cx="390" cy="318" rx="78" ry="52" fill="#5c4a32" stroke="#3d2e1a" stroke-width="2"/>
  <path d="M340 310 C360 292 380 328 400 300 C418 328 440 294 452 318" stroke="#3d2e1a" stroke-width="1.4" fill="none"/>
  <path d="M355 334 C378 348 402 336 424 346" stroke="#4a3a28" stroke-width="2.2" fill="none"/>
  <!-- arms -->
  <path d="M318 308 C280 300 258 278 248 252" stroke="#5c4a32" stroke-width="8" fill="none" stroke-linecap="round"/>
  <path d="M462 300 C510 292 548 270 572 248" stroke="#5c4a32" stroke-width="7" fill="none" stroke-linecap="round"/>
  <!-- whip east, Very Close -->
  <path d="M462 292 C520 260 560 300 548 348 C536 392 500 408 468 390" stroke="#6e8b6e" stroke-width="5" fill="none" stroke-linecap="round"/>
  <path d="M468 390 C452 378 458 362 470 358" stroke="#6e8b6e" stroke-width="3.2" fill="none"/>
  <text x="560" y="336" text-anchor="middle" fill="#9bb394" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">плеть</text>
  <!-- pumpkin head -->
  <circle cx="390" cy="248" r="48" fill="#d4893a" stroke="#3d2e1a" stroke-width="2"/>
  <path d="M390 200 Q404 214 390 226 Q376 214 390 200" fill="#3d6b38" stroke="#3d2e1a" stroke-width="1.2"/>
  <path d="M358 248 Q390 268 422 248" fill="none" stroke="#1a140c" stroke-width="3" stroke-linecap="round"/>
  <ellipse cx="390" cy="256" rx="22" ry="10" fill="#1a140c"/>
  <text x="390" y="244" text-anchor="middle" fill="#1a140c" font-size="11" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">пасть</text>
  <!-- steam cracks -->
  <path d="M368 228 Q364 214 370 204" stroke="#f0d080" stroke-width="1.6" fill="none" opacity="0.85"/>
  <path d="M414 230 Q420 216 412 206" stroke="#f0d080" stroke-width="1.6" fill="none" opacity="0.85"/>
  <text x="390" y="318" text-anchor="middle" fill="#f3ead4" font-size="12" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">джек</text>
  <g><circle cx="348" cy="236" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="348" y="236" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">4</text></g>
  <g><circle cx="422" cy="258" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="422" y="258" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">5</text></g>

  <!-- small pumpkins at the glass, inside -->
  <circle cx="168" cy="128" r="10" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <path d="M168 118 C164 110 172 110 168 118" stroke="#3d6b38" stroke-width="2" fill="none"/>
  <circle cx="250" cy="122" r="9" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="530" cy="124" r="10" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <path d="M530 114 C526 106 534 106 530 114" stroke="#3d6b38" stroke-width="2" fill="none"/>
  <circle cx="612" cy="132" r="9" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="126" cy="250" r="9" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="654" cy="268" r="10" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="160" cy="488" r="9" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="620" cy="484" r="9" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <!-- small pumpkins outside the glass -->
  <circle cx="220" cy="80" r="9" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="390" cy="78" r="10" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <path d="M390 68 C386 60 394 60 390 68" stroke="#3d6b38" stroke-width="2" fill="none"/>
  <circle cx="560" cy="82" r="9" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="716" cy="220" r="10" fill="#d4893a" stroke="#3d2e1a" stroke-width="1.2"/>
  <circle cx="64" cy="300" r="9" fill="#c47a3a" stroke="#3d2e1a" stroke-width="1.2"/>
  <text x="300" y="86" text-anchor="middle" fill="#f3ead4" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">мелкие снаружи</text>
  <g><circle cx="188" cy="122" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="188" y="122" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">6</text></g>

  <!-- cracked glass north + NE -->
  <path d="M200 96 L214 128 L206 160 L228 186" stroke="#f3ead4" stroke-width="1.8" fill="none" opacity="0.8"/>
  <path d="M214 128 L236 120 L248 142" stroke="#f3ead4" stroke-width="1.4" fill="none" opacity="0.7"/>
  <path d="M620 96 L640 140 L628 188 L652 210" stroke="#f3ead4" stroke-width="1.8" fill="none" opacity="0.8"/>
  <path d="M640 140 L668 132" stroke="#f3ead4" stroke-width="1.4" fill="none" opacity="0.7"/>
  <text x="668" y="108" text-anchor="start" fill="#f3ead4" font-size="11" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">стекло</text>
  <g><circle cx="640" cy="118" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="640" y="118" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">2</text></g>

  <!-- south door toward the house -->
  <rect x="350" y="508" width="80" height="18" fill="#6e5a45" stroke="#3d2e1a" stroke-width="1.6"/>
  <rect x="430" y="516" width="22" height="70" rx="2" fill="#8b6b3e" stroke="#3d2e1a" stroke-width="1.6" transform="rotate(28 430 516)"/>
  <text x="390" y="552" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">дверь → дом</text>
  <text x="390" y="570" text-anchor="middle" fill="#dcc9a0" font-size="11" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">вход в Close</text>
  <g><circle cx="338" cy="520" r="12" fill="#d4893a" stroke="#f3ead4" stroke-width="1.6"/><text x="338" y="520" text-anchor="middle" dominant-baseline="central" fill="#1a140c" font-size="13" font-weight="700" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">1</text></g>
  <path d="M390 586 L390 628" stroke="#f0d080" stroke-width="2" stroke-dasharray="6 5"/>
  <text x="404" y="620" text-anchor="start" fill="#f0d080" font-size="12" font-weight="500" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">к дому, не впритык</text>

  <!-- zone key -->
  <rect x="120" y="648" width="540" height="88" rx="6" fill="#243028" stroke="#5c4a32" stroke-width="1.6"/>
  <text x="390" y="672" text-anchor="middle" fill="#f3ead4" font-size="13" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">зоны от джека, не клетки</text>
  <text x="390" y="694" text-anchor="middle" fill="#d4893a" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Melee — корни, тёплый пресс</text>
  <text x="390" y="712" text-anchor="middle" fill="#f0d080" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Very Close — заливка в пасть, плеть</text>
  <text x="390" y="730" text-anchor="middle" fill="#9bb394" font-size="12" font-weight="600" font-family="system-ui, 'Noto Sans', 'DejaVu Sans', sans-serif">Close — грядки, дверь, стекло, мелкие</text>
</svg>

**Легенда**

1. Дверь юг — к дому; открывается в Close. Триггер 1, если группа входит.
2. Стекло и каркас — трещины; ход «дождь стекла» / «ломает теплицу».
3. Грядки — по бокам; северная смята корнями.
4. Джек — голова-тыква, тело из корней, плеть на восток. Стоит в центре, занимает теплицу. Melee — корни.
5. Пасть — заливка фляги из Very Close (состояние 2 или сразу после Major+).
6. Мелкие у стекла — внутри у рам и снаружи; база 4 + свита, здесь где стоят, не сколько.

**Зоны (от джека, не клетки).** Melee — корни, тёплый пресс. Very Close — заливка в пасть, плеть-стебель. Close — грядки, дверь, всё стекло, мелкие у рам. Дальше стекла во двор — уже к дому; Far на этом плане нет.

---

## 4. Промпты для изображений

Скопировать английский блок в ChatGPT (DALL·E). Строки «стиль» и negative при желании дописать в конец того же запроса. Карты сверху — без людей. Кадры мест — сцены, не портреты.

### Карты сверху

#### Рыжий Лог

```
Top-down tabletop RPG game map of a small Halloween village called Ryzhiy Log at night, labeled like a GM battle map, no characters, no people, no animals. A dirt cart track with deep ruts comes from the south through dark crop fields. A huge dark shadow crosses the track and stretches into the fields — only a shadow, no creature drawn. Warm yellow windows of the inn "Svezhaya Pyshka" face the northbound road that leads to the agronomist's estate; a timber stable sits directly beside the inn, with the guild wagon and a horse parked inside, not on the street. Festival square with a few tents and scrawny pumpkins a short walk from the inn. Closed blacksmith and seamstress shops with shutters and X-marked doors. Agronomist Ursag Korneplod's farmstead on the northern outskirts, several minutes away, not next to the square. North arrow. Readable map labels. Calm night colors, pumpkin orange and wood brown. Not photorealistic, not gore, not a painted scene — a clear labeled plan.
```

стиль: top-down tabletop RPG game map, Halloween village, labeled, night, painted, not photoreal, not gore  
negative: no photorealism, no people, no characters, no creatures, no blood, no isometric 3D city render

#### Усадьба Урсага

```
Top-down tabletop RPG game map of agronomist Ursag Korneplod's farmstead at night, labeled like a GM battle map, no characters, no people, no hamster. A wooden fence around the yard. South gate facing the road to town, a guild cart parked just inside the gate. A gnawed hole in the west fence opening to the fields. A barn on the west with its door left ajar. A farmhouse in the center with a porch on the south, a small burrow under the porch, and a ground-level cellar window on the north wall. A well in the yard. Alkali barrels by the house wall. A greenhouse further north of the house, not touching it, with a huge pumpkin filling the glasshouse. North arrow. Readable map labels. Calm night colors, pumpkin orange, glass green, and wood brown. Not photorealistic, not gore, not a painted scene — a clear labeled plan.
```

стиль: top-down tabletop RPG game map, Halloween farmstead, labeled, night, painted, not photoreal, not gore  
negative: no photorealism, no people, no characters, no creatures, no blood

#### Дом Урсага внутри

```
Top-down tabletop RPG floor plan of agronomist Ursag Korneplod's house interior at night, two levels labeled like a GM map, no characters, no people. Upper level: south porch with a burrow underneath, a hall with stairs down, a study with a desk and records, a pantry with jars, a seed packet, and a tiny pumpkin on a shelf. Lower cellar level: a north ground-level window aimed at a greenhouse corner, a brewing cauldron and hearth, a press, a post with a sack tied to it, a supply shelf of old bottles, a barrel and a guild crate. North arrow. Readable Russian-style map labels in English. Calm night cellar colors, pumpkin orange and wood brown. Not photorealistic, not gore, not a painted scene — a clear labeled plan.
```

стиль: top-down tabletop RPG floor plan, house interior and cellar, labeled, night, painted, not photoreal, not gore  
negative: no photorealism, no people, no characters, no creatures, no blood

#### Теплица (зоны)

```
Top-down tabletop RPG game map of agronomist Ursag Korneplod's greenhouse at night, labeled like a GM battle map, Daggerheart range zones not a 5-foot grid. A rectangular glasshouse with a south door facing the farmhouse (house not in frame). Cracked glass panes, wooden frame, a roof ridge line. Raised planting beds along the east and west walls; the north bed crushed. In the center an anthropomorphic Halloween Jack seen from above: huge pumpkin head with a living mouth, bulky torso of tangled roots, root arms and legs, one long vine-whip to the east. Concentric range rings labeled Melee on the roots, Very Close around the mouth and whip, Close out to the glass. Small living pumpkins (walking squash with vine-legs, not people) clustered at the glass inside and just outside. North arrow. Readable map labels. Calm night colors, pumpkin orange, glass green, wood brown. Not photorealistic, not gore, not a painted scene — a clear labeled plan.
```

стиль: top-down tabletop RPG game map, greenhouse battle map, Daggerheart zones, labeled, night, painted, not photoreal, not gore  
negative: no photorealism, no 5-foot grid, no squares, no people, no hamster, no blood

### Кадры мест

Не портреты — кадры места. Тон: comedy horror Halloween, no gore, dusk/evening. Скопировать английский блок в ChatGPT (DALL·E).

#### Погоня

```
Painted tabletop RPG location shot, comedy-horror Halloween, no gore. Camera from the EDGE of a moving guild wagon: the wagon itself is almost out of frame, only a sliver of wooden sideboard and a wheel rim at the bottom of the picture. Evening dusk, not night — amber sky, first distant lanterns ahead. A dirt cart-track with deep ruts runs through tall cornfields on both sides. A pack of many thin field wolves that look like hungry dogs, not direwolves, run alongside and leap at the unseen cart; lots of them, eyes in the corn, barking. No giant hamster, no huge creature in the foreground; if a distant shadow crosses the far field it is tiny and unreadable. No blood, no combat freeze-frame. Painted illustration, not photorealistic.
```

стиль: tabletop RPG location shot, comedy horror Halloween, dusk, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no giant hamster close-up, no night-black sky, no characters in focus, no full wagon filling the frame

#### Гостиница «Свежая Пышка»

```
Painted tabletop RPG location shot of a small-town halfling inn called Svezhaya Pyshka at Halloween dusk, comedy-horror wholesome, no gore. The inn itself is round and low, pumpkin-colored plaster, flour-dusted windows, festival paper lanterns, a hanging sign with a bun. DIRECTLY BESIDE the inn stands a timber barn-stable: the guild wagon with cargo crates is parked inside and a horse is stalled there — not left on the street. Festival town cobbles, a few scrawny pumpkins, evening light not deep night. No portrait; if figures appear they are tiny background silhouettes. Painted illustration, not photorealistic, not gore.
```

стиль: tabletop RPG location shot, Halloween festival town, halfling inn and stable, dusk, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no wagon parked on the street, no character portrait, no deep night

#### Фестиваль на площади

```
Painted tabletop RPG location shot of Ryzhiy Log town square during the Pumpkinwin festival at dusk, comedy-horror Halloween, no gore, not a fight. Tents and stalls, paper lanterns, two rows of scrawny homegrown pumpkins. Townsfolk in homemade Halloween costumes: a giant apple, a paper candle, a straw scarecrow, a barrel with a tap, a too-long dragging cloak, a tiny five-cardboard-dragon-head hoop. The pumpkin-carver's tent of Stameska the wooden clank carpenter: a low stool, a pile of scrawny pumpkins, polished unused carving knives, no one being attacked. Festive and a bit pathetic because the pumpkins are small. Evening golden lantern light. Painted illustration, not photorealistic, not gore, no combat.
```

стиль: tabletop RPG location shot, Halloween festival square, dusk, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no combat, no living attacking pumpkins, no character portrait close-up

#### Усадьба Урсага снаружи

```
Painted tabletop RPG location shot of agronomist Ursag Korneplod's farmstead seen from outside at Halloween dusk, comedy-horror, no gore. Wooden fence, a gate on the road, a barn, the farmhouse, and a greenhouse a little farther behind the house not touching it, crop fields around. Quiet and a bit wrong: the barn door is ajar, a chewed hole in the fence, a well in the yard. Evening, lantern light in the house windows, greenhouse glass catching the last light. No people in the yard. Painted illustration, not photorealistic, not gore.
```

стиль: tabletop RPG location shot, Halloween farmstead exterior, dusk, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no people, no giant hamster, no combat, no character portrait

#### Подвал

```
Painted tabletop RPG location shot of a farm cellar at Halloween evening, comedy-horror, no gore. A brewing cauldron over a hearth with steam, a wooden press, a post with a sack tied to it, a supply shelf of old bottles, a ground-level window showing the corner of a greenhouse outside. Optional: a tired grey-green orc agronomist in a stained leather apron, exhausted after three sleepless nights, not scary, not injured, not a portrait close-up. Warm cellar lantern light. Painted illustration, not photorealistic, not gore, no blood.
```

стиль: tabletop RPG location shot, Halloween farm cellar, brewing, evening, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no horror monster, no character portrait filling the frame

#### Теплица

```
Painted tabletop RPG location shot of a cracked glass greenhouse at Halloween night, comedy-horror, no gore. Inside, an anthropomorphic Halloween Jack plant-giant fills the glasshouse: a huge pumpkin for a head on a bulky torso of tangled roots and vines; arms and legs made of thick roots; one long vine-whip arm coiled like a lash. A clearly visible living mouth on the pumpkin head, large enough to pour a potion flask into — a Halloween Jack grin of rind, not a cute carved lantern, not triangle eyes. Thick armored orange hide, cracks leaking warm steam. Raised planting beds along the glass; small living pumpkins (walking squash with short vine-legs, not people, not humanoid) clustered at the glass inside and just outside. South wooden door toward a farmhouse out of frame. Moonlight through cracked panes, broken glass on the soil. No people, not a hamster. Painted illustration, not photorealistic, not gore.
```

стиль: tabletop RPG location shot, Halloween greenhouse, anthropomorphic pumpkin Jack, night, painted, not photoreal, not gore  
negative: no photorealism, no blood, no gore, no hamster, no cute triangle-eye lantern, no people, no 5-foot grid
