const defaultProjects = [
  {
    id: "landing-auto",
    title: "Лендинг для автосервиса",
    type: "Лендинг",
    category: "landing",
    price: "от 7 000 ₽",
    time: "2–4 дня",
    preview: "Auto Service",
    description: "Демо-сайт для услуги автосервиса с заявкой, блоками преимуществ, ценами и контактами.",
    tasks: ["Первый экран с оффером", "Блок услуг и цен", "Форма заявки", "Адаптация под телефон"],
    stack: ["HTML", "CSS", "JavaScript"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "b2b-catalog",
    title: "B2B каталог товаров",
    type: "Каталог",
    category: "catalog",
    price: "от 18 000 ₽",
    time: "5–10 дней",
    preview: "B2B Catalog",
    description: "Каталог товаров для B2B-продаж: категории, карточки товаров, корзина-заявка и контакты менеджера.",
    tasks: ["Категории товаров", "Карточки с характеристиками", "Корзина-заявка", "Структура под SEO"],
    stack: ["HTML", "CSS", "JavaScript", "CMS-ready"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "telegram-lead-bot",
    title: "Telegram-бот для заявок",
    type: "Telegram-бот",
    category: "bot",
    price: "от 10 000 ₽",
    time: "2–6 дней",
    preview: "Telegram Bot",
    description: "Бот с меню, кнопками, заявками, цепочкой сообщений и возможностью подключить оплату или CRM.",
    tasks: ["Стартовое меню", "Кнопки и разделы", "Сбор заявок", "Простая воронка"],
    stack: ["Python", "Telegram Bot API", "SQLite"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "wordpress-business",
    title: "WordPress сайт компании",
    type: "WordPress",
    category: "wordpress",
    price: "от 6 000 ₽",
    time: "1–5 дней",
    preview: "WordPress",
    description: "Настройка WordPress-сайта: тема, страницы, формы, плагины, домен и базовая структура.",
    tasks: ["Установка WordPress", "Настройка темы", "Формы заявок", "Базовая SEO-настройка"],
    stack: ["WordPress", "Plugins", "CSS"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "news-parser",
    title: "Парсер новостей",
    type: "Автоматизация",
    category: "automation",
    price: "от 5 000 ₽",
    time: "2–7 дней",
    preview: "News Parser",
    description: "Скрипт или сайт, который собирает новости по теме, помогает переводить и готовить публикации.",
    tasks: ["Сбор данных", "Обработка текста", "Фильтрация материалов", "Экспорт результата"],
    stack: ["Python", "Requests", "BeautifulSoup"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "mini-app",
    title: "Telegram Mini App",
    type: "Мини-приложение",
    category: "app",
    price: "от 15 000 ₽",
    time: "5–12 дней",
    preview: "Mini App",
    description: "Мини-приложение для Telegram или браузера: интерфейс, логика, формы и интеграция с ботом.",
    tasks: ["Мобильный интерфейс", "Логика действий", "Интеграция с Telegram", "Подготовка к запуску"],
    stack: ["HTML", "CSS", "JavaScript", "Telegram WebApp"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "web-game",
    title: "Браузерная мини-игра",
    type: "Мини-игра",
    category: "game",
    price: "от 12 000 ₽",
    time: "4–10 дней",
    preview: "Web Game",
    description: "Простая мини-игра для сайта, Telegram, промо-акции или портфолио.",
    tasks: ["Игровая механика", "Экран результата", "Счёт", "Адаптация под телефон"],
    stack: ["JavaScript", "Canvas", "HTML", "CSS"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  },
  {
    id: "code-fix",
    title: "Доработка сайта или кода",
    type: "Правки",
    category: "code",
    price: "от 1 500 ₽",
    time: "от 1 дня",
    preview: "Code Fix",
    description: "Исправление ошибок, адаптива, кнопок, форм, блоков, API или небольших функций.",
    tasks: ["Поиск ошибки", "Исправление кода", "Проверка результата", "Краткое объяснение"],
    stack: ["HTML", "CSS", "JavaScript", "Python", "PHP"],
    demo: "#",
    github: "https://github.com/sharauttxt"
  }
];

const services = [
  {title:"Лендинги",price:"от 7 000 ₽",text:"Одностраничные сайты для заявок, рекламы и быстрого запуска."},
  {title:"Сайты-визитки",price:"от 8 000 ₽",text:"Сайт для специалиста, мастера, компании или личного бренда."},
  {title:"Каталоги товаров",price:"от 18 000 ₽",text:"Категории, карточки, корзина-заявка и удобная структура."},
  {title:"Telegram-боты",price:"от 10 000 ₽",text:"Кнопки, меню, заявки, рассылки, лид-магниты и простая автоматизация."},
  {title:"WordPress",price:"от 6 000 ₽",text:"Установка, настройка, правки, темы, плагины и перенос сайта."},
  {title:"Парсеры",price:"от 5 000 ₽",text:"Сбор данных, обработка файлов, автоматизация повторяющихся действий."},
  {title:"Мини-приложения",price:"от 15 000 ₽",text:"Простые веб-сервисы, Telegram Mini Apps и MVP."},
  {title:"Мини-игры",price:"от 12 000 ₽",text:"Браузерные игры, промо-игры и игровые прототипы."},
  {title:"Доработка кода",price:"от 1 500 ₽",text:"Исправление ошибок, адаптива, форм, блоков и функций."},
  {title:"API и интеграции",price:"от 8 000 ₽",text:"Подключение сервисов, заявок, Telegram, таблиц и внешних API."},
  {title:"Аудит сайта",price:"от 2 000 ₽",text:"Проверка ошибок, адаптива, скорости, структуры и базовых проблем сайта."},
  {title:"Верстка по макету",price:"от 5 000 ₽",text:"Аккуратная адаптивная верстка по Figma, скриншоту или описанию."}
];

const menu = document.querySelector("#menu");
const burger = document.querySelector("#burger");
const modal = document.querySelector("#modal");
const modalContent = document.querySelector("#modalContent");

if (burger) burger.addEventListener("click", () => menu.classList.toggle("open"));
if (menu) menu.querySelectorAll("a").forEach(a => a.addEventListener("click", () => menu.classList.remove("open")));

function getProjects() {
  const local = JSON.parse(localStorage.getItem("atlasProjects") || "[]");
  return [...defaultProjects, ...local];
}

function renderProjects() {
  const grid = document.querySelector("#projectsGrid");
  if (!grid) return;

  const searchInput = document.querySelector("#searchInput");
  const filters = document.querySelectorAll("#filters button");
  let activeFilter = "all";

  function draw() {
    const q = (searchInput?.value || "").toLowerCase().trim();
    const list = getProjects().filter(project => {
      const byFilter = activeFilter === "all" || project.category === activeFilter;
      const bySearch = !q || [project.title, project.type, project.description, project.preview].join(" ").toLowerCase().includes(q);
      return byFilter && bySearch;
    });

    grid.innerHTML = list.map(project => `
      <article class="project-card">
        <div class="project-preview">${project.preview || project.type}</div>
        <div class="project-body">
          <span class="tag">${project.type}</span>
          <h3>${project.title}</h3>
          <p>${project.description}</p>
          <div class="project-meta">
            <span>${project.price || "цена по задаче"}</span>
            <span>${project.time || "срок по задаче"}</span>
          </div>
          <div class="card-actions">
            <button class="small-btn" onclick="openProject('${project.id}')">Подробнее</button>
            <a class="small-btn" href="${project.demo || "#"}" target="_blank" rel="noopener">Ссылка</a>
          </div>
        </div>
      </article>
    `).join("") || `<div class="note-box"><h3>Ничего не найдено</h3><p>Попробуй изменить поиск или фильтр.</p></div>`;
  }

  filters.forEach(btn => btn.addEventListener("click", () => {
    filters.forEach(b => b.classList.remove("active"));
    btn.classList.add("active");
    activeFilter = btn.dataset.filter;
    draw();
  }));

  if (searchInput) searchInput.addEventListener("input", draw);
  draw();
}

function openProject(id) {
  const project = getProjects().find(p => p.id === id);
  if (!project || !modal || !modalContent) return;

  modalContent.innerHTML = `
    <span class="tag">${project.type}</span>
    <h2>${project.title}</h2>
    <p>${project.description}</p>
    <div class="project-meta">
      <span>${project.price || "цена по задаче"}</span>
      <span>${project.time || "срок по задаче"}</span>
    </div>
    <ul>${(project.tasks || []).map(task => `<li>${task}</li>`).join("")}</ul>
    <div class="stack">${(project.stack || []).map(item => `<span>${item}</span>`).join("")}</div>
    <div class="card-actions">
      <a class="btn primary" href="${project.demo || "#"}" target="_blank" rel="noopener">Открыть работу</a>
      <a class="btn ghost" href="${project.github || "https://github.com/sharauttxt"}" target="_blank" rel="noopener">GitHub / кейс</a>
    </div>
  `;
  modal.classList.add("open");
}

document.addEventListener("click", e => {
  if (e.target.dataset.close !== undefined) modal?.classList.remove("open");
});
document.addEventListener("keydown", e => {
  if (e.key === "Escape") modal?.classList.remove("open");
});

function renderServices() {
  const grid = document.querySelector("#servicesGrid");
  const table = document.querySelector("#priceTable");

  if (grid) {
    grid.innerHTML = services.map((s, i) => `
      <article class="service-card">
        <b>${String(i + 1).padStart(2, "0")}</b>
        <h3>${s.title}</h3>
        <p>${s.text}</p>
        <strong>${s.price}</strong>
      </article>
    `).join("");
  }

  if (table) {
    table.innerHTML = services.map(s => `
      <div class="price-row">
        <b>${s.title}</b>
        <strong>${s.price}</strong>
        <p>${s.text}</p>
      </div>
    `).join("");
  }
}

function initBrief() {
  const form = document.querySelector("#briefForm");
  const output = document.querySelector("#briefOutput");
  const copyBtn = document.querySelector("#copyBrief");
  const telegram = document.querySelector("#sendTelegram");
  const mail = document.querySelector("#sendMail");
  if (!form || !output) return;

  form.addEventListener("submit", e => {
    e.preventDefault();
    const data = new FormData(form);

    const message = `Здравствуйте! Хочу обсудить проект.

Имя / компания: ${data.get("name") || "не указано"}
Контакт: ${data.get("contact") || "не указан"}
Что нужно: ${data.get("service") || "не указано"}
Бюджет: ${data.get("budget") || "не указан"}
Срок: ${data.get("deadline") || "не указан"}

Описание задачи:
${data.get("details") || "не указано"}`;

    output.value = message;

    const encoded = encodeURIComponent(message);
    telegram.href = `https://t.me/meekww?text=${encoded}`;
    mail.href = `mailto:skoskr8@gmail.com?subject=${encodeURIComponent("Заявка с Atlas Portfolio")}&body=${encoded}`;
  });

  copyBtn?.addEventListener("click", async () => {
    if (!output.value.trim()) return alert("Сначала соберите сообщение.");
    await navigator.clipboard.writeText(output.value);
    alert("Сообщение скопировано.");
  });
}

renderProjects();
renderServices();
initBrief();
