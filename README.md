# 🛒 Catálogo Digital WhatsApp - Sítio Progresso

Solução web responsiva para catálogo de produtos com carrinho inteligente e integração nativa WhatsApp. Substitui PDFs estáticos por experiência mobile-first.

## 🎯 O Problema
Produtores rurais enviavam catálogos em PDF com centenas de itens. Clientes enfrentavam dificuldades: visualização ruim no celular, cálculo manual de totais, digitação de pedidos no WhatsApp propensa a erros.

## ✅ A Solução
SPA (Single Page Application) leve, sem backend, que funciona como um app nativo:

- **Catálogo Organizado:** Categorias (Citrus, Frutíferas, Ornamentais, Nativas) com busca e filtros
- **Carrinho Lateral:** Adição/remoção de quantidades, cálculo automático de subtotais e total geral
- **Integração WhatsApp One-Click:** Gera mensagem formatada com itens, quantidades, totais e observações — abre direto no WhatsApp Web/App
- **Mobile-First:** Touch-friendly, carrega instantaneamente, funciona offline (Service Worker)
- **Zero Backend:** HTML/CSS/JS puro, hospedagem gratuita no Vercel/GitHub Pages

## 🛠️ Tecnologias
- **HTML5 Semântico** — Acessível, SEO-ready
- **CSS3 Moderno** — Grid/Flexbox, Custom Properties, Media Queries
- **JavaScript ES6+** — Módulos, localStorage para persistência de carrinho
- **WhatsApp Web API** — `wa.me` deep links com mensagem pré-formatada
- **Vercel** — Deploy global, HTTPS, CDN

## 🚀 Como Usar

### Acesso Direto
🔗 **Live:** https://catalogo-digital-whatsapp-omega.vercel.app

### Desenvolvimento Local
```bash
git clone https://github.com/adrianogdr/catalogo-digital-whatsapp.git
cd catalogo-digital-whatsapp
# Abra index.html no browser ou:
npx serve .
```

### Personalização
Edite `index.html` → array `catalogo` com seus produtos:
```javascript
const catalogo = [
  { categoria: "🍊 SUAS CATEGORIAS", itens: [
    { n: "Seu Produto", p: 29.90 },
    // ...
  ]}
];
```

## 📱 Funcionalidades
✨ **Categorias Expansíveis** — Acordeão para navegação limpa  
🛒 **Carrinho Persistente** — Sobrevive a reload (localStorage)  
💰 **Cálculo Automático** — Subtotais + total em tempo real  
📲 **WhatsApp Integrado** — Mensagem pronta: "2x Laranja = R$ 54,00"  
📴 **Offline-First** — Service Worker para cache  
🌙 **Dark Mode** — Segue preferência do sistema  

## 📂 Estrutura
```
catalogo-digital-whatsapp/
├── index.html          # App completo (HTML + CSS + JS inline)
├── vercel.json         # Config deploy Vercel
└── README.md
```

## 🌐 Deploy
**Vercel (1-clique):**
1. Import `adrianogdr/catalogo-digital-whatsapp`
2. Framework: **Other** | Build: *(vazio)* | Output: `.`
3. Deploy → `https://catalogo-digital-whatsapp-omega.vercel.app`

## 👨‍💻 Desenvolvido por
[Adriano Gonçalves](https://github.com/adrianogdr)

## 📄 Licença
MIT — Livre para uso comercial e adaptação.

---

⭐ **Útil para seu negócio? Deixe uma estrela!**