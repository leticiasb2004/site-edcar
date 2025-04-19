<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Oficina Edcar</title>

  <!-- Bootstrap 5 -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" rel="stylesheet">

  <style>
    :root {
      --principal: #0a0e30;
    }

    body {
      font-family: Arial, sans-serif;
    }

    .navbar {
      background-color: var(--principal);
    }

    .hero {
      background: url('https://images.unsplash.com/photo-1587049352839-f674d5b7db63') center/cover no-repeat;
      color: white;
      padding: 100px 0;
      text-align: center;
    }

    .btn-destaque {
      background-color: #ff9900;
      border: none;
      color: white;
      padding: 12px 25px;
      margin-top: 20px;
      border-radius: 5px;
    }

    footer {
      background-color: var(--principal);
      color: #fff;
      text-align: center;
      padding: 20px 0;
    }

    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      z-index: 999;
    }

    .whatsapp-float img {
      width: 60px;
      height: 60px;
    }

    .social-links a {
      color: #fff;
      margin: 0 10px;
      font-size: 1.5rem;
    }

    .mapa iframe {
      width: 100%;
      height: 300px;
      border: none;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark fixed-top">
    <div class="container">
    <a class="navbar-brand" href="#">
  <img src="logomarca.png" alt="Logo Edcar" height="60">
</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#servicos">Serviços</a></li>
          <li class="nav-item"><a class="nav-link" href="#sobre">Sobre</a></li>
          <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="container">
	<font color="#000000">
      <h1>Confiança e Qualidade</h1>
      <p class="lead">A Edcar é sua parceira em manutenção automotiva</p>
	  </font>
      <a href="#servicos" class="btn btn-destaque">Nossos Serviços</a>
    </div>
  </section>

  <!-- Serviços -->
  <section id="servicos" class="py-5">
    <div class="container">
      <h2 class="text-center mb-5">Serviços</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <h5>Revisão Completa</h5>
          <p>Check-up completo com diagnóstico profissional.</p>
        </div>
        <div class="col-md-4">
          <h5>Freios e Suspensão</h5>
          <p>Manutenção com peças de qualidade e mão de obra especializada.</p>
        </div>
        <div class="col-md-4">
          <h5>Troca de Óleo</h5>
          <p>Serviço rápido com lubrificantes das melhores marcas.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Sobre -->
<section id="sobre" class="bg-light py-5">
  <div class="container text-center">
    <h2>Sobre a Oficina Edcar</h2>
    <p class="mt-3">Há mais de 10 anos cuidando do seu carro com excelência em Pará de Minas. Qualidade, transparência e compromisso com você.</p>

    <!-- Carrossel -->
    <div id="carouselSobre" class="carousel slide mt-4" data-bs-ride="carousel">
      <div class="carousel-inner rounded shadow">

        <div class="carousel-item active">
          <img src="foto4.jpg" class="d-block w-100" alt="Foto da oficina 1">
        </div>

        <div class="carousel-item">
          <img src="foto3.jpg" class="d-block w-100" alt="Foto da oficina 2">
        </div>

        <div class="carousel-item">
          <img src="foto1.jpg" class="d-block w-100" alt="Foto da oficina 3">
        </div>

      </div>

      <!-- Botões de navegação -->
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselSobre" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Anterior</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselSobre" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Próximo</span>
      </button>
    </div>
  </div>
</section>


  <!-- Contato -->
  <section id="contato" class="py-5">
    <div class="container">
      <h2 class="text-center mb-4">Fale Conosco</h2>
      <form action="https://api.whatsapp.com/send" method="GET" target="_blank" class="row g-3">
        <input type="hidden" name="phone" value="5537999172576">
        <div class="col-md-6">
          <input type="text" class="form-control" name="nome" placeholder="Seu nome" required>
        </div>
        <div class="col-md-6">
          <input type="email" class="form-control" name="email" placeholder="Seu e-mail" required>
        </div>
        <div class="col-12">
          <textarea class="form-control" name="text" rows="4" placeholder="Escreva sua mensagem aqui" required></textarea>
        </div>
        <div class="col-12 text-center">
          <button type="submit" class="btn btn-success">Enviar via WhatsApp</button>
        </div>
      </form>
    </div>
  </section>

  <!-- Mapa -->
  <section class="mapa my-5">
    <div class="container">
      <h2 class="text-center mb-4">Como Chegar</h2>
      <iframe src="https://www.google.com/maps?q=R.+Geraldo+Alves+da+Silva,+25+-+Dom+Bosco,+Par%C3%A1+de+Minas+-+MG,+35661-353&output=embed" allowfullscreen loading="lazy"></iframe>
    </div>
  </section>

  <!-- Rodapé -->
 <!-- Agendamento de Revisão -->
<section id="agendamento" class="py-5 bg-light">
  <div class="container">
    <h2 class="text-center mb-4">Agende Sua Revisão</h2>
    <form onsubmit="enviarWhatsApp(event)" class="row g-3">
      <div class="col-md-6">
        <input type="text" id="nome" class="form-control" placeholder="Seu nome completo" required>
      </div>
      <div class="col-md-6">
        <input type="tel" id="telefone" class="form-control" placeholder="Seu telefone" required>
      </div>
      <div class="col-md-6">
        <input type="date" id="data" class="form-control" required>
      </div>
      <div class="col-md-6">
        <select id="servico" class="form-select" required>
          <option selected disabled value="">Tipo de serviço</option>
          <option>Revisão completa</option>
          <option>Troca de óleo</option>
          <option>Freios e suspensão</option>
          <option>Outro</option>
        </select>
      </div>
      <div class="col-12 text-center">
        <button type="submit" class="btn btn-success">Agendar via WhatsApp</button>
      </div>
    </form>
  </div>
</section>

 <!-- Contato com Setores -->
<section id="setores" class="py-5 bg-light">
  <div class="container text-center">
    <h2 class="mb-4">Fale com um Setor Específico</h2>
    <div class="row justify-content-center">
      <!-- Financeiro -->
      <div class="col-md-4 mb-3">
        <div class="card h-100 shadow border-0">
          <div class="card-body">
            <h5 class="card-title">Financeiro</h5>
            <p class="card-text">Dúvidas sobre pagamentos, boletos ou cobranças? Fale diretamente com nosso financeiro.</p>
            <a href="https://wa.me/5537999172576" target="_blank" class="btn btn-success">
              <i class="bi bi-whatsapp"></i> Chamar no WhatsApp
            </a>
          </div>
        </div>
      </div>

      <!-- Casa de Peças -->
      <div class="col-md-4 mb-3">
        <div class="card h-100 shadow border-0">
          <div class="card-body">
            <h5 class="card-title">Casa de Peças</h5>
            <p class="card-text">Precisa de peças automotivas ou tem dúvidas sobre disponibilidade?</p>
            <a href="https://wa.me/553799755701" target="_blank" class="btn btn-success">
              <i class="bi bi-whatsapp"></i> Chamar no WhatsApp
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

 <footer>
    <div class="container">
      <p class="mb-2">&copy; 2025 Oficina Edcar - Todos os direitos reservados</p>
      <div class="social-links">
        <a href="https://instagram.com/oficinaedcar_pm" target="_blank"><i class="bi bi-instagram"></i></a>
        <a href="https://wa.me/5537999172576" target="_blank"><i class="bi bi-whatsapp"></i></a>
      </div>
    </div>
  </footer>

  <!-- Botão flutuante do WhatsApp -->
  <a href="https://wa.me/5537999172576" class="whatsapp-float" target="_blank">
    <img src="https://img.icons8.com/color/96/whatsapp--v1.png" alt="WhatsApp">
  </a>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
<script>
  function enviarWhatsApp(event) {
    event.preventDefault();

    const nome = document.getElementById("nome").value;
    const telefone = document.getElementById("telefone").value;
    const data = document.getElementById("data").value;
    const servico = document.getElementById("servico").value;

    const mensagem = `Olá, meu nome é ${nome}%0AQuero agendar uma revisão.%0ATelefone: ${telefone}%0AData: ${data}%0AServiço: ${servico}`;
    const numero = "5537999172576"; // WhatsApp da Oficina Edcar

    const url = `https://wa.me/${numero}?text=${mensagem}`;
    window.open(url, '_blank');
  }
</script>

</body>
</html>
