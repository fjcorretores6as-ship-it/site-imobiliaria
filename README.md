# site-imobilia<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>FJ Corretores — Imóveis em Itapema</title>
  <meta name="description" content="FJ Corretores - Imobiliária em Itapema, Perequê e litoral de Santa Catarina. Casas, apartamentos e lançamentos. Fale no WhatsApp: (47) 9 9253-8545" />
  <style>
    :root{
      --ocean:#0b7bbf;
      --dark:#012a3a;
      --muted:#6b7b86;
      --accent:#ffd166;
      --bg:#f6fbfd;
      --card:#ffffff;
      --radius:12px;
      font-family: Inter, Arial, Helvetica, sans-serif;
    }
    *{box-sizing:border-box}
    body{margin:0;background:var(--bg);color:var(--dark);-webkit-font-smoothing:antialiased}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 28px;background:linear-gradient(90deg,var(--ocean),#0679a8);color:#fff}
    .nav .left{display:flex;align-items:center;gap:18px}
    .brand span{font-weight:700;letter-spacing:1px;color:#fff}
    .menu a{color:rgba(255,255,255,0.95);text-decoration:none;margin:0 10px;font-weight:600}
    .whats{background:#25D366;padding:9px 14px;border-radius:8px;color:#012a3a;text-decoration:none;font-weight:700}
    .hero{background-image:url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1400&q=60');background-size:cover;background-position:center;color:#fff;padding:70px 20px;text-align:center}
    .hero .wrap{max-width:1100px;margin:0 auto}
    .hero h1{margin:0;font-size:36px;text-shadow:0 6px 24px rgba(0,0,0,0.35)}
    .hero p{margin:12px 0 22px;font-size:18px}
    .cta{display:inline-block;background:var(--accent);color:#023047;padding:12px 18px;border-radius:30px;text-decoration:none;font-weight:700}
    .container{max-width:1100px;margin:36px auto;padding:0 18px}
    h2{color:var(--dark);margin-bottom:16px}
    .search{display:flex;gap:10px;margin-bottom:18px;flex-wrap:wrap}
    .search input,.search select{flex:1;padding:12px;border-radius:10px;border:1px solid #e3eef6;background:white}
    .search button{background:var(--ocean);color:white;padding:12px 18px;border-radius:10px;border:none;font-weight:700}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:18px}
    .card{background:var(--card);border-radius:var(--radius);overflow:hidden;box-shadow:0 6px 20px rgba(2,46,68,0.08);display:flex;flex-direction:column}
    .card .thumb{height:180px;background-size:cover;background-position:center}
    .card .body{padding:14px;flex:1;display:flex;flex-direction:column}
    .card h3{margin:0 0 6px;color:var(--ocean)}
    .card p{margin:0 0 10px;color:var(--muted);font-size:14px}
    .card .meta{margin-top:auto;display:flex;justify-content:space-between;align-items:center}
    .btn{background:var(--ocean);color:#fff;padding:8px 12px;border-radius:8px;text-decoration:none;font-weight:700}
    .detail{background:white;padding:22px;border-radius:12px;box-shadow:0 8px 30px rgba(2,46,68,0.06)}
    .gallery{display:flex;gap:10px;margin-bottom:12px}
    .gallery img{width:100%;height:360px;object-fit:cover;border-radius:10px}
    footer{background:var(--dark);color:#fff;padding:30px 18px;margin-top:36px;text-align:center}
    footer p{margin:6px 0;color:rgba(255,255,255,0.9)}
    @media (max-width:720px){.hero h1{font-size:28px}.gallery{flex-direction:column}}
  </style>
</head>
<body>

  <header class="nav">
    <div class="left">
      <div class="brand"><span>FJ CORRETORES</span></div>
      <nav class="menu">
        <a href="#home">Início</a>
        <a href="#imoveis">Imóveis</a>
        <a href="#sobre">Sobre</a>
        <a href="#servicos">Serviços</a>
        <a href="#contato">Contato</a>
      </nav>
    </div>
    <a class="whats" href="https://wa.me/5547992538545" target="_blank">WhatsApp</a>
  </header>

  <section id="home" class="hero">
    <div class="wrap">
      <h1>FJ Corretores — Imóveis em Itapema e litoral de Santa Catarina</h1>
      <p>Casas, apartamentos, lançamentos e oportunidades de investimento. Atendimento personalizado e credibilidade local.</p>
      <a class="cta" href="#imoveis">Ver imóveis</a>
    </div>
  </section>

  <main class="container">
    <section id="imoveis">
      <h2>Catálogo de Imóveis</h2>

      <div class="search">
        <input id="q" placeholder="Buscar por bairro, tipo ou palavra-chave" />
        <select id="tipo"><option value="">Tipo</option><option>Apartamento</option><option>Duplex</option><option>Casa</option></select>
        <select id="bairro"><option value="">Bairro</option><option>Perequê</option><option>Meia Praia</option><option>Itapema</option></select>
        <button id="buscar">Pesquisar</button>
      </div>

      <div id="grid" class="grid"></div>
    </section>

    <section id="lancamentos" style="margin-top:36px">
      <h2>Lançamentos</h2>
      <p>Fique atento: novos empreendimentos em Itapema e Porto Belo. Entre em contato para condições especiais.</p>
    </section>

    <section id="sobre" style="margin-top:36px">
      <h2>Sobre a FJ Corretores</h2>
      <p>A FJ Corretores é uma imobiliária com atuação em Itapema, Perequê e região. Atendemos compradores, investidores e proprietários com transparência e profissionalismo. Nosso time entrega soluções desde avaliação até pós-venda.</p>
    </section>

    <section id="servicos" style="margin-top:36px">
      <h2>Serviços</h2>
      <ul>
        <li>Venda e compra de imóveis</li>
        <li>Intermediação de lançamentos</li>
        <li>Avaliação e consultoria para investidores</li>
        <li>Gestão de temporada</li>
      </ul>
    </section>

  </main>

  <div id="modal" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.6);align-items:center;justify-content:center;padding:20px;z-index:60">
    <div id="modalCard" style="max-width:900px;width:100%;background:white;border-radius:12px;padding:18px;overflow:auto;max-height:90vh"></div>
  </div>

  <section class="container" id="contato">
    <div class="detail">
      <h2>Contato</h2>
      <p>Fale com nossa equipe via WhatsApp ou envie um e-mail.</p>
      <p>WhatsApp: <a href="https://wa.me/5547992538545">(47) 9 9253-8545</a></p>
      <p>E-mail: <a href="mailto:fjcorretores6as@gmail.com">fjcorretores6as@gmail.com</a></p>
      <p>CRECI/SC 10842-J</p>
    </div>
  </section>

  <footer>
    <p>© 2025 FJ Corretores — Itapema / SC</p>
    <p>CRECI/SC 10842-J · WhatsApp: <a href="https://wa.me/5547992538545" style="color:var(--accent);text-decoration:none">(47) 9 9253-8545</a></p>
  </footer>

  <script>
    const properties = [
      { id:'duplex-pereque', title:'Duplex em Perequê', price:'R$ 840.000', area:'90 m²', neighborhood:'Perequê', type:'Duplex', images:['https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?auto=format&fit=crop&w=1200&q=60'], description:'Duplex a 300m do mar. 2 quartos, sala ampla, varanda, excelente investimento.'},
      { id:'rivermouth-apto', title:'Apartamento RiVERMOUTH', price:'R$ 626.000', area:'75 m²', neighborhood:'Perequê', type:'Apartamento', images:['https://images.unsplash.com/photo-1580587771525-78b9dba3b914?auto=format&fit=crop&w=1200&q=60'], description:'600m da praia. Entrada facilitada. 2 por andar.'}
    ];

    const grid = document.getElementById('grid');
    const modal = document.getElementById('modal');
    const modalCard = document.getElementById('modalCard');

    function render(props){
      grid.innerHTML = '';
      props.forEach(p=>{
        const el = document.createElement('article');
        el.className = 'card';
        el.innerHTML = `
          <div class="thumb" style="background-image:url('${p.images[0]}')"></div>
          <div class="body">
            <h3>${p.title}</h3>
            <p>${p.neighborhood} · ${p.area}</p>
            <div class="meta">
              <strong>${p.price}</strong>
              <div style="display:flex;gap:8px">
                <a class="btn" href="#" data-id="${p.id}" onclick="openDetail(event,'${p.id}')">Ver</a>
                <a class="btn" href="https://wa.me/5547992538545?text=Olá!%20Tenho%20interesse%20no%20imóvel%20${encodeURIComponent(p.title)}" target="_blank">WhatsApp</a>
              </div>
            </div>
          </div>
        `;
        grid.appendChild(el);
      });
    }

    function openDetail(e,id){
      e.preventDefault();
      const p = properties.find(x=>x.id===id);
      modalCard.innerHTML = `
        <div style="display:flex;gap:18px;flex-wrap:wrap">
          <div style="flex:1;min-width:260px">
            <div class="gallery"><img src="${p.images[0]}" alt="${p.title}"></div>
          </div>
          <div style="flex:1;min-width:260px">
            <h2>${p.title}</h2>
            <p style="color:var(--muted)">${p.neighborhood} · ${p.area}</p>
            <h3 style="color:var(--ocean)">${p.price}</h3>
            <p>${p.description}</p>
            <p><strong>Tipo:</strong> ${p.type}</p>
            <p style="margin-top:12px"><a class="btn" href="https://wa.me/5547992538545?text=Ol%C3%A1!%20Quero%20mais%20informa%C3%A7%C3%B5es%20sobre%20o%20im%C3%B3vel%20${encodeURIComponent(p.title)}" target="_blank">Enviar WhatsApp</a></p>
            <p style="margin-top:6px"><a href="#" onclick="closeModal()">Fechar</a></p>
          </div>
        </div>
      `;
      modal.style.display = 'flex';
    }
    function closeModal(){modal.style.display='none'}
    document.getElementById('buscar').addEventListener('click',()=>{
      const q = document.getElementById('q').value.toLowerCase();
      const tipo = document.getElementById('tipo').value;
      const bairro = document.getElementById('bairro').value;
      const res = properties.filter(p=>{
        if(tipo && p.type !== tipo) return false;
        if(bairro && p.neighborhood !== bairro) return false;
        if(q && !(p.title.toLowerCase().includes(q) || p.description.toLowerCase().includes(q) || p.neighborhood.toLowerCase().includes(q))) return false;
        return true;
      });
      render(res);
    });
    render(properties);
    modal.addEventListener('click', (e)=>{ if(e.target===modal) closeModal(); })
  </script>
</body>
</html>
ria
