<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Frostpédia — Página principal</title>
<style>
:root{--bg:#f4f8fb;--card:#fff;--ink:#16222d;--mute:#5b6b79;--line:#cfdde8;--acc:#1f6fa8;--acc2:#e6f1f9;--head:#d8eaf6;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0e161d;--card:#15212b;--ink:#e3edf5;--mute:#93a5b5;--line:#2a3b49;--acc:#7cc0f0;--acc2:#1a2d3b;--head:#1d3446}}
:root[data-theme="dark"]{--bg:#0e161d;--card:#15212b;--ink:#e3edf5;--mute:#93a5b5;--line:#2a3b49;--acc:#7cc0f0;--acc2:#1a2d3b;--head:#1d3446}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font:16px/1.6 system-ui,-apple-system,"Segoe UI",sans-serif}
a{color:var(--acc);text-decoration:none}a:hover{text-decoration:underline}
h1,h2,h3{font-family:Georgia,"Times New Roman",serif;font-weight:600;margin:0}
header{background:linear-gradient(135deg,#0f3552,#1f6fa8);color:#fff;padding:20px 16px;text-align:center}
header h1{font-size:2rem;letter-spacing:.5px}header p{margin:4px 0 14px;opacity:.85}
.search{display:flex;max-width:480px;margin:0 auto;gap:6px}
.search input{flex:1;padding:10px 12px;border:0;border-radius:6px;font:inherit}
.search button{padding:10px 14px;border:0;border-radius:6px;background:#0a2438;color:#fff;font:inherit}
nav.top{display:flex;flex-wrap:wrap;gap:6px 18px;justify-content:center;background:var(--card);border-bottom:1px solid var(--line);padding:10px 16px;font-size:.92rem}
main{max-width:1040px;margin:0 auto;padding:16px;display:grid;grid-template-columns:1fr;gap:16px}
@media(min-width:820px){main{grid-template-columns:2fr 1fr}}
.box{background:var(--card);border:1px solid var(--line);border-radius:8px;overflow:hidden}
.box>h2{background:var(--head);padding:8px 14px;font-size:1.1rem;border-bottom:1px solid var(--line)}
.box>div{padding:12px 14px}
.box p{margin:0 0 10px}
.span{grid-column:1/-1}
.welcome{text-align:center}.welcome h2{font-size:1.5rem;margin-bottom:6px}
.stats{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;margin-top:10px}
.stat{background:var(--acc2);border-radius:8px;padding:8px 16px;min-width:120px}
.stat b{display:block;font:600 1.4rem Georgia,serif;color:var(--acc)}.stat small{color:var(--mute)}
.portals{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:10px}
.portal{background:var(--acc2);border-radius:8px;padding:10px 12px}
.portal b{display:block}.portal span{font-size:.85rem;color:var(--mute)}
.people{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:10px}
.person{border:1px solid var(--line);border-radius:8px;padding:10px}
.person b{display:block}.person small{color:var(--mute)}
.tl{margin:0;padding:0;list-style:none;border-left:2px solid var(--line)}
.tl li{padding:0 0 10px 14px;position:relative}
.tl li:before{content:"";position:absolute;left:-6px;top:8px;width:10px;height:10px;border-radius:50%;background:var(--acc)}
.tl b{color:var(--acc)}
.info{width:100%;border-collapse:collapse;font-size:.92rem}
.info td{padding:5px 0;border-bottom:1px solid var(--line);vertical-align:top}.info td:first-child{color:var(--mute);width:42%}
.cats{display:flex;flex-wrap:wrap;gap:6px}.cats a{background:var(--acc2);border-radius:999px;padding:3px 12px;font-size:.88rem}
footer{text-align:center;color:var(--mute);font-size:.85rem;padding:16px}
[hidden]{display:none!important}
.crumb{font-size:.9rem;color:var(--mute);margin-bottom:4px}
.ptitle{font-size:2rem;border-bottom:1px solid var(--line);padding-bottom:6px;margin-bottom:6px}
.ptitle small{display:block;font:400 .95rem system-ui,sans-serif;color:var(--mute)}
.todo{border:1px dashed var(--acc);background:var(--acc2);border-radius:8px;padding:10px 12px;color:var(--mute);margin:0 0 10px}
.todo:before{content:"A PREENCHER";display:inline-block;background:var(--acc);color:var(--card);font:700 .68rem system-ui,sans-serif;border-radius:4px;padding:1px 6px;margin-right:8px;vertical-align:middle}
.art h2{font-size:1.4rem;border-bottom:1px solid var(--line);padding-bottom:4px;margin:44px 0 16px}
.art h3{font-size:1.1rem;margin:26px 0 8px}
.art p{margin:0 0 14px}.art .todo,.art table{margin-bottom:18px}
.art table{width:100%;border-collapse:collapse;font-size:.95rem;margin-bottom:18px}
.art th,.art td{border:1px solid var(--line);padding:6px 10px;text-align:left;vertical-align:top}.art th{background:var(--acc2)}
.pinfo .img{height:190px;display:grid;place-items:center;font-size:3rem;background:linear-gradient(135deg,#0f3552,#5ec4ff);color:#fff;border-radius:6px;margin-bottom:10px}
.pinfo .cap{text-align:center;color:var(--mute);font-size:.85rem;margin-bottom:8px}
.pinfo td:first-child{width:40%}
.toc{background:var(--acc2);border-radius:8px;padding:8px 14px;display:inline-block;font-size:.92rem;margin-bottom:6px}
.toc a{display:block}
@media(max-width:819px){.pinfo{order:-1}}

:root.fd{--bg:#0d1821;--card:#14232f;--ink:#e4edf4;--mute:#92a6b6;--line:#26394a;--acc:#4fb6f2;--acc2:#1a3042;--head:#1c3345}
#p-magnus{max-width:1100px}
#p-magnus .ptitle{font-size:2.3rem;border:0;margin:0}
#p-magnus .ptitle small{display:none}
#p-magnus .crumb a{color:var(--acc)}
.fdart{background:transparent;border:0}
.fdart>div{padding:0}
.fdart p{margin:0 0 14px;line-height:1.7}
.fdart sup{font-size:.7rem}.fdart sup a{color:var(--acc)}
.fdart h2{font-size:1.55rem;border-bottom:1px solid var(--line);padding-bottom:5px;margin:46px 0 16px}
.fdart h3{font-size:1.15rem;margin:28px 0 8px;color:var(--acc)}
.fdart h3 span{font:400 .85rem system-ui,sans-serif;color:var(--mute);margin-left:6px}
.fdart .toc{background:var(--card);border:1px solid var(--line);border-radius:6px;padding:10px 18px;min-width:230px}
.fdart .toc a{margin:2px 0}.fdart .toc a.s{margin-left:16px;font-size:.88rem;color:var(--mute)}
.fdart .def p{margin:0 0 10px}.fdart .def b{color:var(--acc)}
.fdart ul{margin:0 0 14px;padding-left:22px}
.fdart .gal{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:10px}
.fdart .gal div{aspect-ratio:1;border:1px dashed var(--acc);border-radius:6px;background:var(--acc2);display:grid;place-items:center;text-align:center;font-size:.8rem;color:var(--mute);padding:8px}
.fdart ol{padding-left:22px;font-size:.92rem;color:var(--mute)}
.pi{background:var(--card);border:1px solid var(--line);border-radius:6px;overflow:hidden}
.pi .t{background:linear-gradient(135deg,#0f3552,#1d6ea6);color:#fff;text-align:center;font:600 1.3rem Georgia,serif;padding:12px 8px}
.pi .img{height:230px;display:grid;place-items:center;font-size:3.6rem;background:linear-gradient(160deg,#0a2236,#2c86c4);color:#fff}
.pi .cap{text-align:center;color:var(--mute);font-size:.8rem;padding:4px 0 8px;border-bottom:1px solid var(--line)}
.pi .g{background:var(--head);font:700 .78rem system-ui,sans-serif;letter-spacing:.08em;text-transform:uppercase;padding:6px 12px;color:var(--acc)}
.pi .r{display:flex;gap:10px;padding:6px 12px;border-bottom:1px solid var(--line);font-size:.9rem}
.pi .r b{flex:0 0 38%;color:var(--mute);font-weight:600}.pi .r span{flex:1}
.nav{border:1px solid var(--line);border-radius:6px;overflow:hidden;margin-top:34px;font-size:.9rem}
.nav .h{background:linear-gradient(135deg,#0f3552,#1d6ea6);color:#fff;text-align:center;font-weight:600;padding:6px}
.nav .row{display:flex;border-top:1px solid var(--line)}.nav .row b{flex:0 0 150px;background:var(--head);padding:6px 10px;color:var(--acc)}.nav .row span{flex:1;padding:6px 10px}
.catbar{margin-top:16px;border:1px solid var(--line);border-radius:6px;padding:8px 12px;font-size:.88rem;color:var(--mute)}
.catbar a{margin-left:10px}
</style>
</head>
<body>
<header>
  <h1>❄️ Frostpédia</h1>
  <p>A enciclopédia livre da Família Frost e do Gelo Amaldiçoado</p>
  <form class="search" onsubmit="return false"><input id="q" type="search" placeholder="Pesquisar na Frostpédia" aria-label="Pesquisar" autocomplete="off"><button type="button" id="clr">Limpar</button></form>
  <div id="msg" style="margin-top:8px;font-size:.9rem;min-height:1.2em"></div>
</header>
<main id="home">
  <div>
    <section class="box" id="destaque" style="margin-bottom:16px"><h2>⭐ Artigo em destaque: A Criofênix</h2><div>
      <p>A Criofênix é uma criatura lendária e única do gelo, de penas e asas que refletem os tons das auroras austrais. Ela não pertence a ninguém e escolhe livremente a quem acompanhar: o bruxo com mais poder, sabedoria, autocontrole e capacidade de proteger o clã.</p>
      <p>Por tradição, quem recebe sua escolha se torna Patriarca ou Matriarca dos Frost. Foi a Criofênix, por exemplo, que oficializou Magnus como o atual líder. É também a única criatura capaz de conter o avanço do <a href="#">Gelo Amaldiçoado</a>. <a href="#">Leia mais…</a></p>
    </div></section>

    <section class="box" id="portais" style="margin-bottom:16px"><h2>📚 Portais</h2><div class="portals">
      <a class="portal" href="#"><b>A Origem</b><span>Tuniq, Oymyakon e a travessia</span></a>
      <a class="portal" href="#"><b>Caverna Criiko</b><span>O oásis sob o gelo e seu lago</span></a>
      <a class="portal" href="#"><b>Gelo Amaldiçoado</b><span>E a relíquia de Criolita</span></a>
      <a class="portal" href="#"><b>Afinidade Mágica</b><span>Aura gélida e criaturas glaciais</span></a>
      <a class="portal" href="#"><b>Longevidade</b><span>As três etapas do envelhecer</span></a>
      <a class="portal" href="#"><b>Ecos de Criiko</b><span>Memórias nas paredes de cristal</span></a>
    </div></section>

    <section class="box" id="pessoas"><h2>👥 Membros em destaque</h2><div class="people">
      <a class="person" href="#"><b>Anya</b><small>Matriarca fundadora, 1ª geração</small></a>
      <a class="person" href="#/magnus-frost"><b>Magnus Frost</b><small>Patriarca atual e alquimista</small></a>
      <a class="person" href="#"><b>Ellowen Frost</b><small>Guardiã do Polo Sul</small></a>
    </div></section>
  </div>

  <aside>

    <section class="box" style="margin-bottom:16px"><h2>💡 Você sabia?</h2><div>
      <p>Um Frost pode manter a aparência de um jovem de 30 anos mesmo depois de um século de vida.</p>
      <p>Cônjuges bruxos de outras linhagens costumam morrer muito antes dos Frost.</p>
      <p>Aurora abdicou da liderança, convencendo a Criofênix a escolher o irmão Braum.</p>
    </div></section>

    <section class="box" id="cronologia" style="margin-bottom:16px"><h2>🕰️ Cronologia</h2><div>
      <ul class="tl">
        <li><b>Idade Média</b><br>O grupo adota o nome Frost e é expulso de Oymyakon.</li>
        <li><b>Travessia</b><br>Anya lidera a caravela rumo à Antártida e descobre a Caverna Criiko.</li>
        <li><b>3ª geração</b><br>Jack casa-se com Violette Heartsmit e o nome Frost entra na alta sociedade bruxa.</li>
        <li><b>1923</b><br>O acidente criogênico e a morte do Patriarca Cold.</li>
        <li><b>1944</b><br>Magnus cria o bloco de Criolita que sela o Gelo Amaldiçoado.</li>
      </ul>
    </div></section>
  </aside>

  <section class="box span" id="categorias"><h2>🗂️ Categorias</h2><div class="cats">
    <a href="#">Pessoas</a><a href="#">Gerações</a><a href="#">Criaturas</a><a href="#">Locais</a><a href="#">Magia e feitiços</a><a href="#">Poções e alquimia</a><a href="#">Relíquias</a><a href="#">Eventos</a><a href="#">Famílias aliadas</a>
  </div></section>
</main>
<main id="p-magnus" hidden>
  <div class="span"><div class="crumb"><a href="#/">Frostpédia</a> › <a href="#/">Personagens</a> › Magnus Frost</div>
    <h1 class="ptitle">Magnus Frost</h1></div>

  <article class="art box fdart"><div>
    <p><b>Magnus Frost</b> é o atual Patriarca da Família Frost, primogênito de Cold e Priya e irmão de Louis e Ellowen. Mestre alquimista, é o criador das Poções Congeladas, da Poção de Reversão Criogênica e da Criolita moderna, o cristal que sela o Gelo Amaldiçoado.<sup><a href="#r1">[1]</a></sup> É também o único membro do clã que ouve os sussurros do pai, o falecido Patriarca Cold, nas águas do Lago Criiko.<sup><a href="#r1">[1]</a></sup></p>

    <div class="toc"><b>Índice</b>
      <a href="#m-apar">1. Aparência</a><a href="#m-pers">2. Personalidade</a><a href="#m-hist">3. História</a>
      <a class="s" href="#m-h1">3.1 Infância e juventude</a><a class="s" href="#m-h2">3.2 O acidente de 1923</a><a class="s" href="#m-h3">3.3 Patriarca do clã</a><a class="s" href="#m-h4">3.4 A Criolita e os dois polos</a><a class="s" href="#m-h5">3.5 Alquimia e expansão</a><a class="s" href="#m-h6">3.6 Família</a><a class="s" href="#m-h7">3.7 Atualidade</a>
      <a href="#m-hab">4. Habilidades</a><a href="#m-equi">5. Equipamentos</a><a href="#m-rel">6. Relacionamentos</a><a href="#m-triv">7. Curiosidades</a><a href="#m-gal">8. Galeria</a><a href="#m-ref">9. Referências</a>
    </div>

    <h2 id="m-apar">Aparência</h2>
    <p>Magnus tem 149 anos, mas aparenta cerca de 50 anos humanos, como é comum entre os Frost de longa idade.<sup><a href="#r1">[1]</a></sup> Como os demais membros do clã, emana uma aura gélida involuntária, com uma leve brisa fria e flocos de neve ao seu redor.<sup><a href="#r1">[1]</a></sup></p>
    <div class="todo">Cabelo, olhos, altura, roupas e traços marcantes. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>

    <h2 id="m-pers">Personalidade</h2>
    <p>Reservado e observador, Magnus aprendeu cedo a controlar o que sentia e a guardar tudo para si. Demonstra afeto de longe: protege, vigia e cuida sem exigir presença de volta.<sup><a href="#r2">[2]</a></sup> Costuma assumir sozinho as responsabilidades da família, o que o levou a carregar um peso que ninguém lhe pediu diretamente.<sup><a href="#r2">[2]</a></sup></p>
    <div class="todo">Manias, defeitos, gostos e desgostos, e como ele reage a conflitos. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip.</div>

    <h2 id="m-hist">História</h2>
    <h3 id="m-h1">Infância e juventude <span>1877 a 1902</span></h3>
    <p>Primogênito, Magnus cresceu isolado na Caverna Criiko e foi preparado cedo para suceder o pai. Aprendeu a ler os cristais das paredes antes de aprender a nadar no lago e decorou os nomes de dezenas de ancestrais antes de ter um amigo da própria idade.<sup><a href="#r2">[2]</a></sup> Tinha 25 anos quando Louis nasceu, e mais tarde veio Ellowen. Nessa época, assumiu o papel de irmão mais velho que protege à distância.<sup><a href="#r2">[2]</a></sup></p>

    <h3 id="m-h2">O acidente de 1923</h3>
    <p>Em 1923, um acidente criogênico congelou Ellowen, então com 18 anos, e o Patriarca Cold morreu no mesmo episódio.<sup><a href="#r1">[1]</a></sup> Magnus mal pôde lamentar o pai: a urgência de salvar a irmã passou a ocupar todo o seu tempo. Viajou atrás de boticários e arquivos, testou combinações em criaturas pequenas e em gelo comum e percebeu o potencial curativo das lágrimas da Criofênix.<sup><a href="#r2">[2]</a></sup> Após dois anos de pesquisas, combinou as lágrimas com as águas do Lago Criiko e criou a primeira Poção de Reversão Criogênica, que devolveu a vida a Ellowen.<sup><a href="#r1">[1]</a></sup></p>

    <h3 id="m-h3">Patriarca do clã</h3>
    <p>Depois de um ano de luto, no qual passou a ouvir a voz do pai ecoando nos cristais do lago, Magnus se reergueu. A Criofênix, que havia notado sua dedicação ao salvar a irmã, o escolheu oficialmente como novo Patriarca.<sup><a href="#r1">[1]</a></sup> Enquanto a mãe, já idosa, não tinha forças para conduzir o clã, ele também passou a receber os anciãos e resolver disputas sobre a extração de minérios.<sup><a href="#r2">[2]</a></sup></p>

    <h3 id="m-h4">A Criolita e os dois polos <span>1944</span></h3>
    <p>Por volta de 1944, Magnus percebeu que o Gelo Amaldiçoado continuava crescendo e que as tatuagens e fragmentos antigos já não bastavam. Sintetizou então um bloco de Criolita maciço, grande o suficiente para selá-lo e transportável.<sup><a href="#r2">[2]</a></sup> O artefato permitiu as longas viagens do clã e a transferência da sede para Porto Rico.<sup><a href="#r1">[1]</a></sup> Desde então, ele divide a vida entre os dois polos, levando o bloco de um para o outro para aliviar o frio acumulado.<sup><a href="#r2">[2]</a></sup></p>

    <h3 id="m-h5">Alquimia e expansão <span>1945 a 1957</span></h3>
    <p>Nos intervalos entre as viagens, Magnus passou a vender poções, reinvestir em ingredientes raros e abrir lojas e estadias. Em 1945, no Japão, curou um elfo doméstico em estado crítico de uma família sagrada, depois de induzi-lo a um coma controlado e trabalhar meses numa fórmula. Como agradecimento, recebeu um carimbo gravado com seu próprio selo e a promessa de contato com as futuras gerações daquela família.<sup><a href="#r2">[2]</a></sup> A fama de suas receitas fez seu nome circular entre alquimistas e boticários de várias regiões.<sup><a href="#r2">[2]</a></sup></p>

    <h3 id="m-h6">Família <span>1958 a 1975</span></h3>
    <p>Magnus conheceu Alana Fox, filha de uma família puro-sangue, e se casou com ela em uma cerimônia pequena. Confiou a ela todo o segredo do clã e viajaram juntos por anos. Tiveram um filho, Alexander, que ficou no Polo Norte para aprender a história do povo.<sup><a href="#r2">[2]</a></sup></p>
    <div class="todo">O desfecho do casamento com Alana, o que aconteceu depois de 1975 e quando o clã se mudou para Porto Rico. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore.</div>

    <h3 id="m-h7">Atualidade</h3>
    <div class="todo">Situação atual de Magnus, planos e conflitos em aberto. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</div>

    <h2 id="m-hab">Habilidades</h2>
    <div class="def">
      <p><b>Alquimia:</b> mestre na criação de poções raras e complexas, entre elas as Poções Congeladas, que usam as águas do Lago Criiko como ingrediente vital.<sup><a href="#r1">[1]</a></sup></p>
      <p><b>Manipulação térmica:</b> como todos os Frost, domina encantamentos de estase e congelamento e tem aptidão para a Transfiguração Complexa e os Feitiços Não-Verbais.<sup><a href="#r1">[1]</a></sup></p>
      <p><b>Ecos de Criiko:</b> é o único que capta a consciência do pai ressoando no ambiente do lago.<sup><a href="#r1">[1]</a></sup></p>
      <p><b>Limitação:</b> não consegue conjurar feitiços que produzam fogo ou calor intenso.<sup><a href="#r1">[1]</a></sup></p>
    </div>
    <div class="todo">Técnicas de combate, feitiços favoritos e poções inéditas. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</div>

    <h2 id="m-equi">Equipamentos</h2>
    <div class="def">
      <p><b>Bloco de Criolita:</b> recipiente que aprisiona o Gelo Amaldiçoado e permite transportá-lo, hoje uma relíquia da família.<sup><a href="#r1">[1]</a></sup></p>
      <p><b>Carimbo com o selo de Magnus:</b> presente da família sagrada do Japão, guardado longe de olhos curiosos.<sup><a href="#r2">[2]</a></sup></p>
    </div>
    <div class="todo">Outros itens, ingredientes e instrumentos. Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque.</div>

    <h2 id="m-rel">Relacionamentos</h2>
    <h3>Família</h3>
    <ul>
      <li><b>Cold Frost</b> (pai): Patriarca falecido, cuja essência se dissolveu no Lago Criiko.</li>
      <li><b>Priya</b> (mãe): vinda de uma família nobre da Índia, esposa de Cold.</li>
      <li><b>Louis Frost</b> (irmão): inventor das Essências Cristalizadas.</li>
      <li><b>Ellowen Frost</b> (irmã): guardiã do Polo Sul, salva por Magnus.</li>
      <li><b>Alana Fox</b> (esposa): de família puro-sangue.</li>
      <li><b>Alexander Frost</b> (filho): criado no Polo Norte.</li>
      <li><b>Zacary Frost</b> (tio): ex-Auror e foragido.</li>
    </ul>
    <h3>Aliados</h3><div class="todo">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</div>
    <h3>Rivais</h3><div class="todo">Ut labore et dolore magna aliqua, quis nostrud exercitation.</div>

    <h2 id="m-triv">Curiosidades</h2>
    <div class="todo">Fatos curiosos e bastidores do personagem. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.</div>

    <h2 id="m-gal">Galeria</h2>
    <div class="gal"><div>Imagem a adicionar<br>Lorem ipsum</div><div>Imagem a adicionar<br>Lorem ipsum</div><div>Imagem a adicionar<br>Lorem ipsum</div><div>Imagem a adicionar<br>Lorem ipsum</div></div>

    <h2 id="m-ref">Referências</h2>
    <ol><li id="r1">Cursed Ice, documento-base da Família Frost.</li><li id="r2">Frozen Black Jesus, memórias de Magnus Frost.</li></ol>

    <div class="nav"><div class="h">Família Frost</div>
      <div class="row"><b>Fundadores</b><span>Anya · Milo</span></div>
      <div class="row"><b>3ª a 4ª geração</b><span>Jack Frost · Violette Heartsmit · Rell Frost · Aldric Frost</span></div>
      <div class="row"><b>6ª geração</b><span>Cold Frost · Zacary Frost</span></div>
      <div class="row"><b>7ª geração</b><span>Magnus Frost · Louis Frost · Ellowen Frost</span></div>
      <div class="row"><b>8ª e 9ª geração</b><span>Alexander · Iris · Kaito e Kione · Theo · Ezran</span></div>
    </div>
    <div class="catbar">Categorias:<a href="#/">Pessoas</a><a href="#/">7ª geração</a><a href="#/">Patriarcas</a><a href="#/">Alquimistas</a><a href="#/">Vivos</a></div>
  </div></article>

  <aside class="pinfo"><div class="pi">
    <div class="t">Magnus Frost</div>
    <div class="img">🧪</div><div class="cap">Imagem a adicionar</div>
    <div class="g">Informações gerais</div>
    <div class="r"><b>Título</b><span>Patriarca do clã Frost</span></div>
    <div class="r"><b>Gênero</b><span>Masculino</span></div>
    <div class="r"><b>Espécie</b><span>Bruxo (linhagem Tuniq-Frost)</span></div>
    <div class="r"><b>Geração</b><span>7ª</span></div>
    <div class="r"><b>Nascimento</b><span>1877</span></div>
    <div class="r"><b>Idade</b><span>149 anos (aparenta cerca de 50)</span></div>
    <div class="r"><b>Residência</b><span>Porto Rico</span></div>
    <div class="r"><b>Ocupação</b><span>Alquimista e dono de loja de poções</span></div>
    <div class="r"><b>Afiliação</b><span>Família Frost</span></div>
    <div class="r"><b>Status</b><span>Vivo</span></div>
    <div class="g">Família</div>
    <div class="r"><b>Pais</b><span>Cold e Priya</span></div>
    <div class="r"><b>Irmãos</b><span>Louis e Ellowen</span></div>
    <div class="r"><b>Cônjuge</b><span>Alana Fox</span></div>
    <div class="r"><b>Filhos</b><span>Alexander</span></div>
    <div class="g">Características</div>
    <div class="r"><b>Cabelo</b><span>Lorem ipsum</span></div>
    <div class="r"><b>Olhos</b><span>Lorem ipsum</span></div>
    <div class="r"><b>Altura</b><span>Lorem ipsum</span></div>
    <div class="g">Aparições</div>
    <div class="r"><b>Primeira aparição</b><span>Lorem ipsum</span></div>
    <div class="r"><b>Criado por</b><span>Lorem ipsum</span></div>
  </div></aside>
</main>
<footer>Frostpédia · Esta enciclopédia está em construção. Ajude a expandi-la criando novas páginas.</footer>
<script>
(function(){
  var q=document.getElementById('q'),msg=document.getElementById('msg');
  var items=[].slice.call(document.querySelectorAll('#home .person,#home .portal,#home .cats a,#home .tl li'));
  var boxes=[].slice.call(document.querySelectorAll('#home .box'));
  function norm(t){return t.toLowerCase().normalize('NFD').replace(/[\u0300-\u036f]/g,'');}
  function run(){
    var v=norm(q.value.trim()),n=0;
    items.forEach(function(el){
      var hit=!v||norm(el.textContent).indexOf(v)>-1;
      el.style.display=hit?'':'none';
      if(v&&hit)n++;
    });
    boxes.forEach(function(b){
      var its=b.querySelectorAll('.person,.portal,.cats a,.tl li');
      if(!v||!its.length){b.style.display='';return;}
      var any=[].some.call(its,function(i){return i.style.display!=='none';});
      b.style.display=any?'':'none';
    });
    msg.textContent=!v?'':(n?n+' resultado'+(n>1?'s':'')+' encontrado'+(n>1?'s':''):'Nenhum resultado para "'+q.value.trim()+'"');
  }
  q.addEventListener('input',function(){if(location.hash.indexOf('#/')===0)location.hash='#/';run();});
  document.getElementById('clr').addEventListener('click',function(){q.value='';run();q.focus();});
})();
</script>
<script>
(function(){
  var home=document.getElementById('home'),pg=document.getElementById('p-magnus');
  function route(){
    var h=location.hash,onPage=h==='#/magnus-frost';
    pg.hidden=!onPage;home.hidden=onPage;document.documentElement.classList.toggle('fd',onPage);
    if(onPage){window.scrollTo(0,0);document.title='Magnus Frost — Frostpédia';}
    else{document.title='Frostpédia — Página principal';
      var t=h.length>1&&h.charAt(1)!=='/'?document.getElementById(h.slice(1)):null;
      if(t)t.scrollIntoView();else window.scrollTo(0,0);}
  }
  window.addEventListener('hashchange',route);route();
})();
</script>
</body>
</html>
