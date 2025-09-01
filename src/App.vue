<template>
  <div id="app">
    <nav
      class="navbar navbar-expand-lg fixed-top"
      :class="{ 'navbar-scrolled': isScrolled }"
    >
      <div class="container">
        <a class="navbar-brand" href="#inicio">
          <img src="@/assets/logo.png" alt="Concepto Logo" height="60" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav" ref="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a
                class="nav-link"
                href="#inicio"
                :class="{ active: activeSection === 'inicio' }"
                @click="closeMobileMenu"
                >Inicio</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#servicios"
                :class="{ active: activeSection === 'servicios' }"
                @click="closeMobileMenu"
                >Servicios</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#pacientes"
                :class="{ active: activeSection === 'pacientes' }"
                @click="closeMobileMenu"
                >Pacientes</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#team"
                :class="{ active: activeSection === 'team' }"
                @click="closeMobileMenu"
                >Team Concepto</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#sedes"
                :class="{ active: activeSection === 'sedes' }"
                @click="closeMobileMenu"
                >Sedes</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="#turnos"
                :class="{ active: activeSection === 'turnos' }"
                @click="closeMobileMenu"
                >Turnos</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <main>
      <section id="inicio">
        <div
          class="container h-100 d-flex flex-column justify-content-center align-items-center text-center text-white"
        >
          <h2 class="text-uppercase small-caps">Concepto Kinésico</h2>
          <h1 class="display-3 fw-bold text-uppercase">
            Rehabilitación<br />Personalizada
          </h1>
          <p class="lead my-4">
            Te ayudamos a recuperar tu movilidad y calidad de vida.<br />
            En cada sesión vas a estar un paso más cerca de tu bienestar.
          </p>
          <a
            href="#turnos"
            class="btn btn-custom-blue btn-lg text-uppercase fw-bold"
            >Solicitar Turno</a
          >
        </div>
      </section>

      <section id="servicios" class="bg-light">
        <div class="container">
          <div class="row text-center mb-5">
            <div class="col-12">
              <h2 class="section-title">SERVICIOS</h2>
              <p class="lead text-secondary">
                Cada cuerpo es único, por eso nuestros tratamientos también lo
                son. Te ofrecemos un plan de rehabilitación a medida, adaptado a
                tus necesidades y objetivos.
              </p>
            </div>
          </div>
          <div class="row">
            <div class="col-lg-3 col-md-6 mb-4">
              <div class="card h-100 shadow-sm text-center">
                <img
                  src="@/assets/servicio-kinesiologia.webp"
                  class="card-img-top"
                  alt="Servicio de Kinesiología"
                />
                <div class="card-body d-flex flex-column">
                  <h5 class="card-title fw-bold">KINESIOLOGÍA</h5>
                  <p class="card-text">
                    Tratamos tu lesión pensando en tus necesidades específicas,
                    buscando que tengas un estilo y calidad de vida más
                    saludable.
                  </p>
                  <a
                    href="#turnos"
                    class="btn btn-custom-blue mt-auto align-self-center"
                    >TURNOS</a
                  >
                </div>
              </div>
            </div>
            <div class="col-lg-3 col-md-6 mb-4">
              <div class="card h-100 shadow-sm text-center">
                <img
                  src="@/assets/servicio-osteopatia.webp"
                  class="card-img-top"
                  alt="Servicio de Osteopatía"
                />
                <div class="card-body d-flex flex-column">
                  <h5 class="card-title fw-bold">OSTEOPATÍA</h5>
                  <p class="card-text">
                    Tratamos tu cuerpo en forma holística, buscando el
                    equilibrio visceral, hormonal, neural, vascular y del
                    sistema nervioso autónomo.
                  </p>
                  <a
                    href="#turnos"
                    class="btn btn-custom-blue mt-auto align-self-center"
                    >TURNOS</a
                  >
                </div>
              </div>
            </div>
            <div class="col-lg-3 col-md-6 mb-4">
              <div class="card h-100 shadow-sm text-center">
                <img
                  src="@/assets/servicio-rpg.webp"
                  class="card-img-top"
                  alt="Servicio de RPG"
                />
                <div class="card-body d-flex flex-column">
                  <h5 class="card-title fw-bold">RPG</h5>
                  <p class="card-text">
                    Tratamos tus problemas posturales en forma global, buscando
                    la salud de tu columna vertebral.
                  </p>
                  <a
                    href="#turnos"
                    class="btn btn-custom-blue mt-auto align-self-center"
                    >TURNOS</a
                  >
                </div>
              </div>
            </div>
            <div class="col-lg-3 col-md-6 mb-4">
              <div class="card h-100 shadow-sm text-center">
                <img
                  src="@/assets/servicio-plantillas.webp"
                  class="card-img-top"
                  alt="Servicio de Plantillas"
                />
                <div class="card-body d-flex flex-column">
                  <h5 class="card-title fw-bold">PLANTILLAS</h5>
                  <p class="card-text">
                    Diseñadas a medida mediante un estudio estático y dinámico
                    de la pisada. Previenen lesiones, corrigen la postura y
                    alivian el dolor.
                  </p>
                  <a
                    href="#turnos"
                    class="btn btn-custom-blue mt-auto align-self-center"
                    >TURNOS</a
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="pacientes" ref="pacientesSection">
        <div class="container">
          <div class="row text-center mb-5">
            <div class="col-lg-8 offset-lg-2">
              <h2 class="section-title-white">NUESTROS PACIENTES</h2>
              <p class="lead">
                Trabajamos mano a mano con deportistas de élite, brindándoles
                tratamientos personalizados y avanzados para que puedan superar
                sus límites y alcanzar sus metas más ambiciosas.
              </p>
            </div>
          </div>
          <div class="row text-center">
            <div class="col-md-4">
              <h1 class="counter-number">
                +{{ Math.floor(pacientesAtendidos) }}
              </h1>
              <p class="counter-label">PACIENTES ATENDIDOS</p>
            </div>
            <div class="col-md-4">
              <h1 class="counter-number">{{ Math.floor(anosExperiencia) }}</h1>
              <p class="counter-label">AÑOS DE EXPERIENCIA</p>
            </div>
            <div class="col-md-4">
              <h1 class="counter-number">{{ Math.floor(deportistasElite) }}</h1>
              <p class="counter-label">DEPORTISTAS DE ELITE</p>
            </div>
          </div>
        </div>
      </section>

      <section id="team">
        <div class="container">
          <div class="row text-center mb-5">
            <div class="col-lg-8 offset-lg-2">
              <h2 class="section-title">TEAM CONCEPTO</h2>
              <p class="lead text-secondary">
                Nuestro equipo de kinesiólogos está compuesto por profesionales
                apasionados que encuentran gran satisfacción en ayudar a otros a
                superar sus desafíos físicos. Con cada paciente, celebramos los
                pequeños triunfos y los grandes avances.
              </p>
            </div>
          </div>
          <div class="row">
            <div class="col-lg-4 text-center mb-5">
              <img
                src="@/assets/team-member-1.webp"
                alt="Lic. Iriel Kotlar"
                class="team-img mb-3"
              />
              <h5 class="team-name">LIC. IRIEL KOTLIAR</h5>
              <div class="team-description">
                <p>
                  Lic. Kinesiología y Fisiatría<br />
                  Osteópata<br />
                  Postgrado Reeducación Postural Global de Cadenas
                  Miofasciales<br />
                  Profesora de Ed. Física
                </p>
              </div>
            </div>
            <div class="col-lg-4 text-center mb-5">
              <img
                src="@/assets/team-member-2.webp"
                alt="Lic. Carla Perez"
                class="team-img mb-3"
              />
              <h5 class="team-name">LIC. CARLA PEREZ</h5>
              <div class="team-description">
                <p>
                  Lic. Kinesiología y Fisiatría<br />
                  Postgrado en Reeducación Postural Global de Cadenas
                  Miofasciales.
                </p>
              </div>
            </div>
            <div class="col-lg-4 text-center mb-5">
              <img
                src="@/assets/team-member-3.webp"
                alt="Lic. Clara Candia"
                class="team-img mb-3"
              />
              <h5 class="team-name">LIC. CLARA CANDIA</h5>
              <div class="team-description">
                <p>Lic. Kinesiología y Fisiatría</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="sedes">
        <div class="container">
          <div class="row text-center mb-5">
            <div class="col-12">
              <h2 class="section-title-white">SEDES</h2>
            </div>
          </div>
          <ul
            class="nav nav-tabs justify-content-center"
            id="sedesTab"
            role="tablist"
          >
            <li class="nav-item" role="presentation">
              <button
                class="nav-link active"
                id="caba-tab"
                data-bs-toggle="tab"
                data-bs-target="#caba"
                type="button"
                role="tab"
                aria-controls="caba"
                aria-selected="true"
              >
                CABA
              </button>
            </li>
            <li class="nav-item" role="presentation">
              <button
                class="nav-link"
                id="vicente-lopez-tab"
                data-bs-toggle="tab"
                data-bs-target="#vicente-lopez"
                type="button"
                role="tab"
                aria-controls="vicente-lopez"
                aria-selected="false"
              >
                VICENTE LÓPEZ
              </button>
            </li>
          </ul>
          <div class="tab-content" id="sedesTabContent">
            <div
              class="tab-pane fade show active"
              id="caba"
              role="tabpanel"
              aria-labelledby="caba-tab"
            >
              <div class="row align-items-center mt-5">
                <div class="col-lg-6">
                  <div class="sede-info">
                    <ul class="list-unstyled">
                      <li>
                        <i class="fas fa-map-marker-alt me-2"></i>ESTADO DE
                        ISRAEL 4156 6to Piso – Club Hacoaj
                      </li>
                      <li>
                        <i class="fas fa-phone-alt me-2"></i>+54 9 11 6022-2345
                      </li>
                      <li>
                        <i class="fas fa-clock me-2"></i>Lunes a Viernes de 8:00
                        a 20:00 hs
                      </li>
                    </ul>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="map-container">
                    <iframe
                      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3284.2444814341957!2d-58.426881525654295!3d-34.59797885719275!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95bcca7b6d750575%3A0x743e7887bc07c0c6!2sAv.%20Estado%20de%20Israel%204156%2C%20C1414%20Cdad.%20Aut%C3%B3noma%20de%20Buenos%20Aires!5e0!3m2!1ses!2sar!4v1753018816702!5m2!1ses!2sar"
                      width="500"
                      height="200"
                      style="border: 0"
                      allowfullscreen=""
                      loading="lazy"
                      referrerpolicy="no-referrer-when-downgrade"
                    ></iframe>
                  </div>
                </div>
              </div>
            </div>
            <div
              class="tab-pane fade"
              id="vicente-lopez"
              role="tabpanel"
              aria-labelledby="vicente-lopez-tab"
            >
              <div class="row align-items-center mt-5">
                <div class="col-lg-6">
                  <div class="sede-info">
                    <ul class="list-unstyled">
                      <li>
                        <i class="fas fa-map-marker-alt me-2"></i>AV. SAN MARTIN
                        1649 – COAT
                      </li>
                      <li>
                        <i class="fas fa-phone-alt me-2"></i>+54 9 11 6022-2345
                      </li>
                      <li>
                        <i class="fas fa-clock me-2"></i>Lunes a Viernes de 8:00
                        a 20:00 hs
                      </li>
                    </ul>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="map-container">
                    <iframe
                      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3287.1346042106893!2d-58.48833332565908!3d-34.52481755333321!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95bcb14a78cad085%3A0xa7082a69c1c186ec!2sJose%20de%20Gral%2C%20Gral.%20Jos%C3%A9%20de%20San%20Mart%C3%ADn%201649%2C%20B1602BWB%20Florida%2C%20Provincia%20de%20Buenos%20Aires%2C%20Argentina!5e0!3m2!1ses!2shr!4v1736871618173!5m2!1ses!2shr"
                      title="SEDE VICENTE LOPEZ"
                      width="500"
                      height="200"
                      style="border: 0"
                      allowfullscreen=""
                      loading="lazy"
                      referrerpolicy="no-referrer-when-downgrade"
                    ></iframe>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="turnos" class="bg-white">
        <div class="container">
          <div class="row text-center mb-5">
            <div class="col-12">
              <h2 class="section-title">TURNOS</h2>
              <p class="lead text-secondary">
                Completa el formulario y te contactaremos por WhatsApp para
                coordinar tu turno.
              </p>
            </div>
          </div>
          <div class="row justify-content-center">
            <div class="col-lg-6">
              <form @submit.prevent="enviarWhatsApp">
                <div class="mb-3">
                  <label for="nombre" class="form-label"
                    >Nombre y Apellido</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="nombre"
                    v-model="form.nombre"
                    required
                  />
                </div>
                <div class="mb-3">
                  <label for="motivo" class="form-label"
                    >Motivo de la consulta</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="motivo"
                    v-model="form.motivo"
                    required
                    placeholder="Ej: Dolor de espalda, rehabilitación, etc."
                  />
                </div>
                <div class="mb-3">
                  <label for="mensaje" class="form-label"
                    >Mensaje (Opcional)</label
                  >
                  <textarea
                    class="form-control"
                    id="mensaje"
                    rows="4"
                    v-model="form.mensaje"
                  ></textarea>
                </div>
                <div class="d-grid">
                  <button type="submit" class="btn btn-whatsapp fw-bold">
                    <i class="fab fa-whatsapp me-2"></i> ENVIAR MENSAJE
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </section>

      <footer id="footer" class="footer-section">
        <div class="container">
          <div class="row align-items-center justify-content-between">
            <div class="col-lg-5 col-md-6 mb-4 mb-md-0">
              <img
                src="@/assets/logo.png"
                alt="Concepto Logo"
                height="50"
                class="footer-logo mb-3"
              />
              <p>
                Centro de kinesiología y rehabilitación personalizada. Te
                ayudamos a recuperar tu movilidad y calidad de vida.
              </p>
            </div>
            <div class="col-lg-5 col-md-6 text-md-end">
              <div class="footer-social">
                <h5>Seguinos en nuestro Instagram</h5>
                <a
                  href="https://www.instagram.com/concepto.kinesico"
                  target="_blank"
                  class="instagram-link"
                >
                  <i class="fab fa-instagram"></i>
                  <span>@concepto.kinesico</span>
                </a>
              </div>
            </div>
          </div>
          <div class="footer-bottom">
            <div class="copyright">
              MCG Solutions © 2025 Concepto Kinésico. Todos los derechos
              reservados.
            </div>
          </div>
        </div>
      </footer>
    </main>
  </div>
</template>

<script>
import { Collapse } from "bootstrap";

export default {
  name: "App",
  data() {
    return {
      isScrolled: false,
      activeSection: "inicio",
      sections: ["inicio", "servicios", "pacientes", "team", "sedes", "turnos"],
      pacientesAtendidos: 0,
      anosExperiencia: 0,
      deportistasElite: 0,
      counterStarted: false,
      form: {
        nombre: "",
        motivo: "",
        mensaje: "",
      },
      menuCollapseInstance: null,
    };
  },
  methods: {
    handleScroll() {
      if (window.scrollY > 50) {
        this.isScrolled = true;
      } else {
        this.isScrolled = false;
      }
      for (const sectionId of this.sections) {
        const section = document.getElementById(sectionId);
        if (section) {
          const rect = section.getBoundingClientRect();
          if (rect.top <= 100 && rect.bottom >= 100) {
            this.activeSection = sectionId;
            break;
          }
        }
      }
    },
    animateCounter(target, dataProperty, duration) {
      const start = this[dataProperty];
      const increment = (target - start) / duration;
      let current = start;
      const timer = setInterval(() => {
        current += increment;
        this[dataProperty] = current;
        if (current >= target) {
          clearInterval(timer);
          this[dataProperty] = target;
        }
      }, 1);
    },
    enviarWhatsApp() {
      const telefono = "5491160222345"; // Reemplaza con tu número

      let mensajeCodificado = `Hola, quiero solicitar un turno.
*Nombre y Apellido:* ${this.form.nombre}
*Motivo:* ${this.form.motivo}
*Mensaje:* ${this.form.mensaje || "No ingresado"}`;

      mensajeCodificado = encodeURIComponent(mensajeCodificado);

      const url = `https://wa.me/${telefono}?text=${mensajeCodificado}`;
      window.open(url, "_blank");
    },
    closeMobileMenu() {
      if (this.menuCollapseInstance && this.menuCollapseInstance._isShown) {
        this.menuCollapseInstance.hide();
      }
    },
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);

    const menuElement = this.$refs.navbarNav;
    this.menuCollapseInstance = new Collapse(menuElement, {
      toggle: false,
    });

    const observer = new IntersectionObserver(
      (entries) => {
        const entry = entries[0];
        if (entry.isIntersecting && !this.counterStarted) {
          this.animateCounter(5345, "pacientesAtendidos", 2000);
          this.animateCounter(20, "anosExperiencia", 2000);
          this.animateCounter(150, "deportistasElite", 2000);
          this.counterStarted = true;
          observer.unobserve(this.$refs.pacientesSection);
        }
      },
      {
        threshold: 0.5,
      }
    );
    observer.observe(this.$refs.pacientesSection);
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.handleScroll);
  },
};
</script>

<style>
/* --- ESTILOS GLOBALES --- */
html {
  scroll-behavior: smooth;
}

/* --- ESTILOS DEL MENÚ DE NAVEGACIÓN (NAVBAR) --- */
.navbar {
  transition: background-color 0.4s ease-in-out, box-shadow 0.4s ease-in-out;
  background-color: transparent !important;
}
.navbar.navbar-scrolled {
  background-color: #ffffff !important;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}
.navbar .nav-link {
  color: white;
  font-weight: 500;
  transition: color 0.3s ease;
}
.navbar.navbar-scrolled .nav-link {
  color: #333;
}
.navbar .nav-link.active,
.navbar.navbar-scrolled .nav-link.active {
  color: #34bbf0 !important;
}
.navbar .nav-link:hover {
  color: #34bbf0 !important;
}
.navbar-scrolled .navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(0, 0, 0, 1)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
}

/* --- ESTILOS DE LA SECCIÓN HERO (INICIO) --- */
#inicio {
  min-height: 100vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.7)),
    url("@/assets/hero-background.webp");
  background-size: cover;
  background-position: center center;
}
.small-caps {
  font-size: 0.9rem;
  font-weight: bold;
  letter-spacing: 0.2rem;
}
.btn-custom-blue {
  background-color: #34bbf0;
  border-color: #34bbf0;
  color: white;
  padding: 12px 30px;
  border-radius: 50px;
  transition: all 0.3s ease;
}
.btn-custom-blue:hover {
  background-color: #2ca8d8;
  border-color: #2ca8d8;
  color: white;
  transform: translateY(-2px);
}

/* --- ESTILOS PARA LAS OTRAS SECCIONES --- */
section {
  padding: 100px 0;
}
.section-title {
  color: #34bbf0;
  font-weight: 700;
  text-transform: uppercase;
  margin-bottom: 20px;
}
.card {
  border: none;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1) !important;
}
.card-title {
  color: #333;
  margin-bottom: 15px;
}
.card-text {
  font-size: 0.9rem;
  color: #6c757d;
}

/* --- ESTILOS RESPONSIVOS PARA EL MENÚ EN MÓVILES --- */
@media (max-width: 991.98px) {
  .navbar {
    background-color: #ffffff !important;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  .navbar .nav-link {
    color: #333 !important;
  }
  .navbar .nav-link.active {
    color: #34bbf0 !important;
  }
  .navbar-nav {
    text-align: right;
  }
  .navbar-toggler-icon {
    background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(0, 0, 0, 1)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e") !important;
  }
}

/* --- ESTILOS PARA LAS IMÁGENES DE SERVICIOS --- */
#servicios .card-img-top {
  height: 200px;
  object-fit: cover;
  width: 100%;
}

/* --- ESTILOS SECCIÓN PACIENTES (CONTADOR) --- */
#pacientes {
  background-color: #212529;
  color: #ffffff;
}
.section-title-white {
  font-weight: 700;
  text-transform: uppercase;
  margin-bottom: 20px;
  color: #ffffff;
}
.counter-number {
  font-size: 4rem;
  font-weight: 700;
}
.counter-label {
  font-size: 1rem;
  letter-spacing: 2px;
  text-transform: uppercase;
}

/* --- ESTILOS SECCIÓN TEAM --- */
.team-img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #f0f0f0;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}
.team-name {
  font-weight: 700;
  color: #333;
  margin-bottom: 10px;
}
.team-description p {
  font-size: 0.9rem;
  color: #6c757d;
  line-height: 1.6;
}

/* --- ESTILOS SECCIÓN SEDES (FORMATO TABS) --- */
#sedes {
  background-color: #212529;
}
.nav-tabs {
  border-bottom: 2px solid #495057;
}
.nav-tabs .nav-link {
  border: none;
  background-color: transparent;
  color: #adb5bd;
  font-weight: 600;
  text-transform: uppercase;
  padding: 10px 20px;
  transition: all 0.3s ease;
}
.nav-tabs .nav-link.active,
.nav-tabs .nav-link:hover {
  color: #34bbf0;
  border-bottom: 2px solid #34bbf0;
}
.nav-tabs .nav-link.active {
  border-color: transparent transparent #34bbf0 transparent;
}
.tab-content {
  padding-top: 20px;
}
.sede-info ul li {
  margin-bottom: 15px;
  color: #f8f9fa;
  display: flex;
  align-items: center;
  font-size: 1rem;
}
.sede-info ul li i {
  color: #34bbf0;
  font-size: 1.2rem;
  width: 25px;
}
.map-container {
  overflow: hidden;
  position: relative;
  height: 0;
  padding-bottom: 75%;
  border-radius: 8px;
}
.map-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}

/* --- ESTILOS SECCIÓN TURNOS (FORMULARIO) --- */
#turnos {
  background-color: #ffffff;
}
.form-label {
  color: #333;
  font-weight: 500;
}
.form-control {
  border-radius: 8px;
  border: 1px solid #ced4da;
  padding: 12px;
}
.form-control:focus {
  border-color: #34bbf0;
  box-shadow: 0 0 0 0.25rem rgba(52, 187, 240, 0.25);
}
.btn-whatsapp {
  background-color: #25d366;
  color: white;
  padding: 15px;
  font-size: 1.1rem;
  border-radius: 50px;
  border: none;
  transition: background-color 0.3s ease;
}
.btn-whatsapp:hover {
  background-color: #1ebe57;
  color: white;
}

/* --- ESTILOS FOOTER --- */
.footer-section {
  background-color: #000000;
  color: #adb5bd;
  padding: 60px 0;
}
.footer-section p {
  margin-bottom: 0;
}
.footer-logo {
  filter: brightness(0) invert(1);
}
.footer-social h5 {
  color: #ffffff;
  font-weight: 600;
  margin-bottom: 15px;
}
.instagram-link {
  display: inline-flex;
  align-items: center;
  font-size: 1.2rem;
  color: #adb5bd;
  text-decoration: none;
  transition: color 0.3s ease;
}
.instagram-link:hover {
  color: #34bbf0;
}
.instagram-link i {
  font-size: 1.8rem;
  margin-right: 10px;
}
.footer-bottom {
  border-top: 1px solid #343a40;
  margin-top: 40px;
  padding-top: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.copyright {
  font-size: 0.9rem;
}
</style>
