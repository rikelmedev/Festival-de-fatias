<h1 align="center">🍰 Festival de Fatias — Cardápio Digital</h1>

<p align="center">
  Cardápio digital estilo <em>app de delivery</em> que monta o pedido e finaliza direto no WhatsApp.<br>
  Feito para a confeitaria <strong>Jessica Raiani Bolos</strong>.
</p>

<p align="center">
  <a href="https://festival-de-fatias-nu.vercel.app/"><strong>🔗 Ver ao vivo</strong></a>
</p>

<p align="center">
  <img alt="HTML5"  src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white">
  <img alt="CSS3"   src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black">
  <img alt="Deploy" src="https://img.shields.io/badge/Deploy-Vercel-000000?style=flat&logo=vercel&logoColor=white">
  <img alt="Sem dependências" src="https://img.shields.io/badge/depend%C3%AAncias-0-brightgreen?style=flat">
</p>

---

## 📖 Sobre o projeto

A confeitaria precisava divulgar os sabores do festival e receber pedidos de forma
organizada, sem depender de um sistema caro. A solução é uma **página única**, leve e
responsiva, onde o cliente:

1. escolhe os sabores e as quantidades (como num carrinho de app de delivery);
2. escolhe entre **entrega** (com taxa) ou **retirada**;
3. informa nome, telefone e endereço;
4. clica em **Finalizar** e a mensagem do pedido é montada e aberta **direto no WhatsApp** da confeitaria.

Tudo em um só arquivo `index.html`, sem back-end e sem banco de dados.

## ✨ Funcionalidades

- 🧁 **15 sabores** com contador de quantidade individual
- 💰 **Cálculo automático** de subtotal, taxa de entrega e total
- 🛵 **Delivery ou retirada** — a taxa e o campo de endereço aparecem conforme a escolha
- 📲 **Pedido pelo WhatsApp** — mensagem formatada gerada automaticamente
- ✅ **Validação** de nome, telefone e endereço antes de enviar
- 🎨 **Banner ilustrado em SVG** — sem depender de imagem externa (nunca "quebra")
- 📱 **100% responsivo** e otimizado para toque em celular

## 💡 Detalhes de UX

- Cards de sabor que **acendem** ao serem selecionados
- **Vibração tátil** (feedback háptico) ao adicionar/remover fatias em celulares compatíveis
- Botão "Finalizar" com **badge de quantidade** e estado **adormecido** quando o carrinho está vazio
- Barra de total fixa com efeito *glass* e animação ao mudar o valor
- Tipografia com **Fraunces** (títulos) e **DM Sans** (corpo)

## 🛠️ Tecnologias

- **HTML5** semântico
- **CSS3** puro (grid, flexbox, variáveis, animações, `backdrop-filter`)
- **JavaScript** (vanilla, sem frameworks nem bibliotecas)
- **Google Fonts** — Fraunces + DM Sans
- Deploy na **Vercel**

> Zero dependências, zero build. É só abrir o `index.html`.

## 🚀 Como executar localmente

```bash
# 1. Clone o repositório
git clone https://github.com/rikelmedev/Festival-de-fatias.git

# 2. Entre na pasta
cd Festival-de-fatias

# 3. Abra o index.html no navegador
#    (ou rode um servidor simples)
python -m http.server 8000
# depois acesse http://localhost:8000
```

## ⚙️ Personalização

As principais configurações ficam no topo do `<script>`, fáceis de ajustar:

```js
const PRICE = 18;                 // preço por fatia (R$)
const DELIVERY_FEE = 4;           // taxa de entrega (R$)
const WHATSAPP = "5517996010156"; // número que recebe os pedidos
const PICKUP_ADDRESS = "...";     // endereço de retirada
```

Para editar os sabores, altere a lista de cards na seção **"Escolha suas fatias"**
e o array `FLAVORS` no script (mantendo a mesma ordem).

## 📂 Estrutura

```
Festival-de-fatias/
├── index.html   # todo o projeto (HTML + CSS + JS em um arquivo)
└── README.md
```

## 👤 Autor

**Rikelme Oliveira**

- GitHub: [@rikelmedev](https://github.com/rikelmedev)

---

<p align="center">Feito com 💜 para adoçar pedidos.</p>
