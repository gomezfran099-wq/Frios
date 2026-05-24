# Frios
Aprende hacer pasteles frios sin experiencia 
<!DOCTYPE html>
<html lang="es-MX">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Especialista en Pasteles Fríos | Aprende y Vende desde Casa</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=DM+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --rosa: #D4537E;
    --rosa-light: #FBEAF0;
    --rosa-dark: #72243E;
    --cafe: #5C3A1E;
    --cafe-light: #8B5E3C;
    --verde: #2D7A4F;
    --crema: #FDF6EE;
    --blanco: #FFFFFF;
    --texto: #2C1A0E;
    --texto-suave: #6B4C35;
    --sombra: 0 4px 24px rgba(44,26,14,0.10);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--crema);
    color: var(--texto);
    line-height: 1.65;
  }

  /* NAV */
  .nav {
    background: var(--blanco);
    padding: 14px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 1px solid #F0E0D0;
  }
  .nav-logo {
    font-family: 'Playfair Display', serif;
    font-size: 17px;
    color: var(--rosa-dark);
    font-weight: 700;
  }
  .nav-cta {
    background: var(--rosa);
    color: var(--blanco);
    border: none;
    padding: 9px 18px;
    border-radius: 30px;
    font-family: 'DM Sans', sans-serif;
    font-size: 13px;
    font-weight: 600;
    cursor: pointer;
    text-decoration: none;
  }

  /* HERO */
  .hero {
    background: linear-gradient(160deg, #FDF0F5 0%, #FDF6EE 60%, #F9EDE0 100%);
    padding: 48px 24px 40px;
    text-align: center;
  }
  .hero-badge {
    display: inline-block;
    background: var(--rosa-light);
    color: var(--rosa-dark);
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 6px 16px;
    border-radius: 20px;
    margin-bottom: 20px;
  }
  .hero h1 {
    font-family: 'Playfair Display', serif;
    font-size: 34px;
    line-height: 1.2;
    color: var(--cafe);
    margin-bottom: 8px;
  }
  .hero h1 span {
    color: var(--rosa);
  }
  .hero-sub {
    font-size: 16px;
    color: var(--texto-suave);
    margin-bottom: 28px;
    max-width: 340px;
    margin-left: auto;
    margin-right: auto;
  }
  .hero-pills {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-bottom: 32px;
    max-width: 340px;
    margin-left: auto;
    margin-right: auto;
  }
  .hero-pill {
    background: var(--cafe);
    color: var(--crema);
    font-size: 14px;
    padding: 10px 20px;
    border-radius: 30px;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .hero-pill::before {
    content: "▶";
    font-size: 10px;
    color: var(--rosa);
  }
  .btn-primary {
    display: block;
    background: #27AE60;
    color: var(--blanco);
    text-decoration: none;
    font-size: 17px;
    font-weight: 700;
    padding: 18px 30px;
    border-radius: 12px;
    text-align: center;
    letter-spacing: 0.02em;
    max-width: 380px;
    margin: 0 auto 16px;
    box-shadow: 0 6px 20px rgba(39,174,96,0.35);
  }
  .hero-precio {
    font-size: 15px;
    color: var(--cafe);
    font-weight: 600;
    margin-bottom: 12px;
  }
  .hero-precio span {
    font-size: 22px;
    color: var(--rosa-dark);
  }
  .hero-precio .msi {
    display: block;
    font-size: 13px;
    color: var(--texto-suave);
    font-weight: 400;
  }
  .hero-garantias {
    display: flex;
    justify-content: center;
    gap: 18px;
    flex-wrap: wrap;
    margin-top: 4px;
  }
  .garantia-item {
    display: flex;
    align-items: center;
    gap: 5px;
    font-size: 12px;
    color: var(--texto-suave);
  }
  .garantia-icon {
    font-size: 16px;
  }

  /* GALERÍA */
  .galeria {
    padding: 40px 24px;
    background: var(--blanco);
  }
  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 24px;
    color: var(--cafe);
    text-align: center;
    margin-bottom: 8px;
  }
  .section-sub {
    text-align: center;
    font-size: 14px;
    color: var(--texto-suave);
    margin-bottom: 24px;
  }
  .galeria-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    max-width: 400px;
    margin: 0 auto;
  }
  .galeria-card {
    background: var(--rosa-light);
    border-radius: 16px;
    padding: 22px 14px;
    text-align: center;
    font-size: 13px;
    font-weight: 500;
    color: var(--rosa-dark);
  }
  .galeria-emoji {
    font-size: 32px;
    display: block;
    margin-bottom: 8px;
  }

  /* PARA QUIÉN */
  .para-quien {
    padding: 40px 24px;
    background: var(--crema);
  }
  .card-check {
    background: var(--blanco);
    border-radius: 16px;
    padding: 18px;
    margin-bottom: 14px;
    display: flex;
    gap: 14px;
    align-items: flex-start;
    box-shadow: var(--sombra);
  }
  .check-icon {
    background: #27AE60;
    color: var(--blanco);
    width: 26px;
    height: 26px;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    flex-shrink: 0;
  }
  .card-check h3 {
    font-size: 15px;
    font-weight: 600;
    color: var(--cafe);
    margin-bottom: 4px;
  }
  .card-check p {
    font-size: 13px;
    color: var(--texto-suave);
    line-height: 1.5;
  }

  /* MÓDULOS */
  .modulos {
    padding: 40px 24px;
    background: var(--blanco);
  }
  .modulo-card {
    border: 1.5px solid #F0DDD0;
    border-radius: 16px;
    padding: 20px;
    margin-bottom: 16px;
  }
  .modulo-num {
    display: inline-block;
    background: var(--rosa-light);
    color: var(--rosa-dark);
    font-size: 11px;
    font-weight: 700;
    padding: 4px 12px;
    border-radius: 20px;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    margin-bottom: 10px;
  }
  .modulo-card h3 {
    font-family: 'Playfair Display', serif;
    font-size: 18px;
    color: var(--rosa);
    margin-bottom: 6px;
  }
  .modulo-card p {
    font-size: 13px;
    color: var(--texto-suave);
    margin-bottom: 12px;
  }
  .modulo-items {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 6px;
  }
  .modulo-items li {
    font-size: 13px;
    color: var(--texto);
    display: flex;
    gap: 8px;
    align-items: flex-start;
  }
  .modulo-items li::before {
    content: "→";
    color: var(--rosa);
    font-weight: 700;
    flex-shrink: 0;
    margin-top: 1px;
  }

  /* ADAPATCIONES MX */
  .adaptaciones {
    padding: 36px 24px;
    background: var(--cafe);
    color: var(--crema);
  }
  .adaptaciones .section-title {
    color: var(--crema);
  }
  .adaptaciones .section-sub {
    color: rgba(253,246,238,0.7);
  }
  .adapt-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    max-width: 400px;
    margin: 0 auto;
  }
  .adapt-card {
    background: rgba(253,246,238,0.08);
    border: 1px solid rgba(253,246,238,0.15);
    border-radius: 14px;
    padding: 16px 14px;
    text-align: center;
  }
  .adapt-card .icon {
    font-size: 24px;
    margin-bottom: 8px;
  }
  .adapt-card h4 {
    font-size: 13px;
    font-weight: 600;
    color: var(--crema);
    margin-bottom: 4px;
  }
  .adapt-card p {
    font-size: 11px;
    color: rgba(253,246,238,0.65);
    line-height: 1.4;
  }

  /* GARANTÍA */
  .garantia {
    padding: 36px 24px;
    background: var(--crema);
    text-align: center;
  }
  .garantia-box {
    background: var(--blanco);
    border-radius: 20px;
    padding: 28px 20px;
    max-width: 380px;
    margin: 0 auto;
    box-shadow: var(--sombra);
    border: 2px solid var(--rosa-light);
  }
  .garantia-seal {
    font-size: 56px;
    margin-bottom: 12px;
  }
  .garantia-box h3 {
    font-family: 'Playfair Display', serif;
    font-size: 22px;
    color: var(--cafe);
    margin-bottom: 10px;
  }
  .garantia-box p {
    font-size: 14px;
    color: var(--texto-suave);
    line-height: 1.6;
  }

  /* CTA FINAL */
  .cta-final {
    padding: 48px 24px;
    background: linear-gradient(160deg, #FDF0F5 0%, #FDF6EE 100%);
    text-align: center;
  }
  .cta-final h2 {
    font-family: 'Playfair Display', serif;
    font-size: 28px;
    color: var(--cafe);
    margin-bottom: 10px;
  }
  .cta-final h2 span {
    color: var(--rosa);
  }
  .cta-final p {
    font-size: 15px;
    color: var(--texto-suave);
    margin-bottom: 28px;
    max-width: 340px;
    margin-left: auto;
    margin-right: auto;
  }
  .precio-bloque {
    background: var(--blanco);
    border-radius: 16px;
    padding: 22px;
    max-width: 360px;
    margin: 0 auto 24px;
    box-shadow: var(--sombra);
  }
  .precio-antes {
    font-size: 14px;
    color: var(--texto-suave);
    text-decoration: line-through;
    margin-bottom: 4px;
  }
  .precio-ahora {
    font-size: 13px;
    color: var(--cafe);
    margin-bottom: 6px;
  }
  .precio-grande {
    font-size: 42px;
    font-weight: 700;
    color: var(--rosa-dark);
    font-family: 'Playfair Display', serif;
    line-height: 1;
    margin-bottom: 4px;
  }
  .precio-msi {
    font-size: 14px;
    color: var(--verde);
    font-weight: 600;
    margin-bottom: 4px;
  }
  .precio-nota {
    font-size: 11px;
    color: var(--texto-suave);
  }

  /* FOOTER */
  .footer {
    background: var(--cafe);
    color: rgba(253,246,238,0.65);
    text-align: center;
    padding: 24px;
    font-size: 12px;
    line-height: 1.8;
  }
  .footer a {
    color: rgba(253,246,238,0.85);
    text-decoration: underline;
  }

  /* Animaciones suaves */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .hero { animation: fadeUp 0.7s ease both; }
</style>
</head>
<body>

<!-- NAV -->
<nav class="nav">
  <div class="nav-logo">🍰 Pasteles Fríos MX</div>
  <a href="#comprar" class="nav-cta">¡Quiero aprender!</a>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-badge">🇲🇽 Especial para México</div>
  <h1>Aprende a hacer y vender <span>pasteles fríos rentables</span>, ¡sin experiencia!</h1>
  <p class="hero-sub">Recetas fáciles con ingredientes que encuentras en Walmart, Chedraui y tienditas. Sin gastar en equipo caro.</p>

  <div class="hero-pills">
    <div class="hero-pill">Sin experiencia previa</div>
    <div class="hero-pill">Empieza con lo que tienes en casa</div>
    <div class="hero-pill">Vende en WhatsApp, Instagram y fiestas</div>
  </div>

  <a href="#comprar" class="btn-primary">🎓 ¡QUIERO APRENDER AHORA!</a>

  <div class="hero-precio">
    Solo <span>$597 MXN</span>
    <span class="msi">o hasta 12 MSI con tu tarjeta</span>
  </div>
  <div class="hero-garantias">
    <div class="garantia-item"><span class="garantia-icon">⚡</span> Acceso inmediato</div>
    <div class="garantia-item"><span class="garantia-icon">🔒</span> Pago seguro</div>
    <div class="garantia-item"><span class="garantia-icon">✅</span> 7 días de garantía</div>
  </div>
</section>

<!-- GALERÍA DE PASTELES -->
<section class="galeria">
  <h2 class="section-title">Pasteles que aprenderás a hacer</h2>
  <p class="section-sub">¡Deliciosos, rentables y perfectos para el mercado mexicano!</p>
  <div class="galeria-grid">
    <div class="galeria-card">
      <span class="galeria-emoji">🍫</span>
      Pastel frío de chocolate con cajeta
    </div>
    <div class="galeria-card">
      <span class="galeria-emoji">🍓</span>
      Pastel de fresas con crema
    </div>
    <div class="galeria-card">
      <span class="galeria-emoji">🥥</span>
      Pastel de coco y leche condensada
    </div>
    <div class="galeria-card">
      <span class="galeria-emoji">🌰</span>
      Pastel de pistache y nuez
    </div>
    <div class="galeria-card">
      <span class="galeria-emoji">🍮</span>
      Pastel de tres leches frío
    </div>
    <div class="galeria-card">
      <span class="galeria-emoji">🍋</span>
      Pastel de limón con merengue
    </div>
  </div>
</section>

<!-- PARA QUIÉN -->
<section class="para-quien">
  <h2 class="section-title">Este curso es perfecto para ti si…</h2>
  <p class="section-sub" style="margin-bottom:28px;">No importa si eres de CDMX, Guadalajara, Veracruz o cualquier rincón de México</p>

  <div class="card-check">
    <div class="check-icon">✓</div>
    <div>
      <h3>Quieres un ingreso extra sin salir de casa</h3>
      <p>Vende a tus vecinos, en grupos de WhatsApp, en la escuela de tus hijos o en fiestas y eventos. Trabaja a tu propio ritmo.</p>
    </div>
  </div>

  <div class="card-check">
    <div class="check-icon">✓</div>
    <div>
      <h3>Eres ama de casa o mamá con tiempo limitado</h3>
      <p>Incorpora la repostería a tu rutina diaria sin necesidad de grandes inversiones ni equipo profesional.</p>
    </div>
  </div>

  <div class="card-check">
    <div class="check-icon">✓</div>
    <div>
      <h3>Ya vendes pasteles y quieres ampliar tu menú</h3>
      <p>Los pasteles fríos tienen altísima demanda en México para XV años, cumpleaños, bodas y eventos. Diferénciate de la competencia.</p>
    </div>
  </div>

  <div class="card-check">
    <div class="check-icon">✓</div>
    <div>
      <h3>Buscas emprender pero no sabes por dónde empezar</h3>
      <p>Aprenderás desde cero: recetas, costos, precios en pesos mexicanos y cómo conseguir tus primeros clientes.</p>
    </div>
  </div>
</section>

<!-- MÓDULOS DEL CURSO -->
<section class="modulos">
  <h2 class="section-title">Lo que aprenderás</h2>
  <p class="section-sub" style="margin-bottom:28px;">De cero a la venta, paso a paso</p>

  <div class="modulo-card">
    <span class="modulo-num">Módulo 1</span>
    <h3>Bases del pastel frío perfecto</h3>
    <p>Todo lo que necesitas saber antes de empezar: herramientas, temperaturas y la lógica del pastel congelado.</p>
    <ul class="modulo-items">
      <li>Equipo básico que ya tienes o consigues en cualquier ferretería</li>
      <li>Cómo almacenar y transportar tus pasteles fríos</li>
      <li>La diferencia entre pastel frío y pastel congelado</li>
    </ul>
  </div>

  <div class="modulo-card">
    <span class="modulo-num">Módulo 2</span>
    <h3>Masas perfectas con ingredientes mexicanos</h3>
    <p>La base de tu pastel es lo que marca la diferencia. Recetas adaptadas con productos de Walmart, Chedraui y La Costco.</p>
    <ul class="modulo-items">
      <li>Bizcocho esponjoso y jugoso (receta completa)</li>
      <li>Pastel de chocolate cremoso — el favorito de todos</li>
      <li>Variante de chocolate negro con sabor intenso</li>
    </ul>
  </div>

  <div class="modulo-card">
    <span class="modulo-num">Módulo 3</span>
    <h3>Rellenos y salsas irresistibles</h3>
    <p>Los rellenos que más venden en México, adaptados con ingredientes locales.</p>
    <ul class="modulo-items">
      <li>Rellenos cremosos: chocolate, cajeta, coco, pistache, fresa</li>
      <li>Mousses de leche y chocolate</li>
      <li>Almíbar de piloncillo, vainilla y canela (toque mexicano)</li>
      <li>Compota de guayaba, mango y maracuyá</li>
    </ul>
  </div>

  <div class="modulo-card">
    <span class="modulo-num">Módulo 4</span>
    <h3>Glasados y decoración profesional</h3>
    <p>El acabado que hace que tus pasteles se vean de pastelería de lujo, aunque los hagas en casa.</p>
    <ul class="modulo-items">
      <li>Glasado espejo (mirror glaze) paso a paso</li>
      <li>Cobertura de chocolate con acabado brillante</li>
      <li>Decoraciones simples con alto impacto visual</li>
      <li>Empaque atractivo para venta y regalo</li>
    </ul>
  </div>

  <div class="modulo-card">
    <span class="modulo-num">Módulo 5</span>
    <h3>Cómo vender y fijar tus precios en pesos</h3>
    <p>La parte que otros cursos ignoran: cómo ganar dinero de verdad con tus pasteles en México.</p>
    <ul class="modulo-items">
      <li>Cálculo de costos con ingredientes mexicanos (precios actualizados)</li>
      <li>Fijación de precios para diferentes mercados: colonia, redes sociales, eventos</li>
      <li>Estrategias de venta por WhatsApp e Instagram</li>
      <li>Cómo conseguir pedidos para XV años, bodas y cumpleaños</li>
    </ul>
  </div>
</section>

<!-- ADAPTACIONES PARA MÉXICO -->
<section class="adaptaciones">
  <h2 class="section-title">100% adaptado para México</h2>
  <p class="section-sub">No es una traducción — es una adaptación real</p>
  <div class="adapt-grid">
    <div class="adapt-card">
      <div class="icon">🛒</div>
      <h4>Ingredientes locales</h4>
      <p>Walmart, Chedraui, Costco y tiendas de materias primas</p>
    </div>
    <div class="adapt-card">
      <div class="icon">💰</div>
      <h4>Precios en MXN</h4>
      <p>Costos y márgenes calculados en pesos mexicanos</p>
    </div>
    <div class="adapt-card">
      <div class="icon">🎉</div>
      <h4>Sabores mexicanos</h4>
      <p>Cajeta, piloncillo, tamarindo, guayaba y más</p>
    </div>
    <div class="adapt-card">
      <div class="icon">📱</div>
      <h4>Venta digital MX</h4>
      <p>WhatsApp, Facebook Marketplace e Instagram shopping</p>
    </div>
    <div class="adapt-card">
      <div class="icon">📦</div>
      <h4>Envíos y logística</h4>
      <p>Cómo usar Rappi, Uber Eats y paqueterías locales</p>
    </div>
    <div class="adapt-card">
      <div class="icon">📋</div>
      <h4>COFEPRIS básico</h4>
      <p>Lo que necesitas saber para vender alimentos legalmente</p>
    </div>
  </div>
</section>

<!-- GARANTÍA -->
<section class="garantia">
  <div class="garantia-box">
    <div class="garantia-seal">🛡️</div>
    <h3>Garantía de 7 días sin preguntas</h3>
    <p>Si en los primeros 7 días después de tu compra sientes que el curso no es lo que esperabas, te devolvemos tu dinero completo. Sin preguntas, sin complicaciones. Puedes pagar con total tranquilidad.</p>
  </div>
</section>

<!-- CTA FINAL -->
<section class="cta-final" id="comprar">
  <h2>¡Empieza tu negocio de <span>pasteles fríos</span> hoy mismo!</h2>
  <p>Acceso inmediato a todos los módulos. Aprende a tu ritmo, desde tu teléfono o computadora.</p>

  <div class="precio-bloque">
    <div class="precio-antes">Precio normal: $997 MXN</div>
    <div class="precio-ahora">Precio de lanzamiento:</div>
    <div class="precio-grande">$597 MXN</div>
    <div class="precio-msi">o 12 MSI desde $49.75/mes</div>
    <div class="precio-nota">Acepta Visa, Mastercard, OXXO, SPEI y PayPal</div>
  </div>

  <a href="#" class="btn-primary">🎓 ¡SÍ, QUIERO APRENDER AHORA!</a>

  <div class="hero-garantias" style="margin-top:16px;">
    <div class="garantia-item"><span class="garantia-icon">⚡</span> Acceso inmediato</div>
    <div class="garantia-item"><span class="garantia-icon">🔒</span> Pago 100% seguro</div>
    <div class="garantia-item"><span class="garantia-icon">✅</span> 7 días de garantía</div>
  </div>
</section>

<!-- FOOTER -->
<footer class="footer">
  <p>Pasteles Fríos MX · Curso digital · Acceso en línea</p>
  <p style="margin-top:6px;">
    <a href="#">Aviso de privacidad</a> · <a href="#">Términos y condiciones</a> · <a href="#">Contacto</a>
  </p>
  <p style="margin-top:8px;">Producto digital. Los resultados pueden variar según el esfuerzo de cada persona.</p>
</footer>

</body>
</html>
