# 🏗️ Flex Container - A Base do Flexbox

O Flexbox é um modelo de layout poderoso no CSS que nos ajuda a organizar elementos de forma flexível e responsiva. Para começar, precisamos entender o **Flex Container**, que é a "elemento pai" onde a magia acontece! ✨

## 📦 O que é um Flex Container?
O **Flex Container** é o elemento pai que abriga os itens flexíveis. Para criar um container flexível, basta definir a propriedade `display: flex;` no elemento pai. Assim, todos os filhos diretos se tornam **Flex Items** automaticamente! 🔥

### 📝 Exemplo básico:
```css
.container {
  display: flex;
  background-color: #f0f0f0;
  padding: 20px;
}
.item {
  background-color: #4caf50;
  color: white;
  padding: 10px;
  margin: 5px;
  border-radius: 5px;
}
```

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

## 🎯 Principais Propriedades do Flex Container
Aqui estão as principais propriedades que podem ser usadas no **Flex Container**:

### 1️⃣ `display: flex;`
Ativa o **Flexbox** e transforma o elemento em um container flexível.

### 2️⃣ `flex-direction`
Define a direção dos itens flexíveis:
- `row` (padrão) ➡️ os itens ficam lado a lado.
- `row-reverse` ⬅️ os itens ficam lado a lado, mas invertidos.
- `column` ⬇️ os itens ficam empilhados verticalmente.
- `column-reverse` ⬆️ os itens ficam empilhados, mas invertidos.

🔹 **Exemplo:**
```css
.container {
  display: flex;
  flex-direction: column;
}
```

### 3️⃣ `justify-content`
Controla o alinhamento dos itens no eixo principal:
- `flex-start` (padrão) 🔜 alinha os itens no início.
- `flex-end` 🔚 alinha os itens no final.
- `center` 🔛 centraliza os itens.
- `space-between` ↔️ espaçamento igual entre os itens.
- `space-around` 🔄 espaçamento ao redor dos itens.
- `space-evenly` 🔀 espaçamento uniforme entre os itens.

🔹 **Exemplo:**
```css
.container {
  display: flex;
  justify-content: center;
}
```

### 4️⃣ `align-items`
Alinha os itens no eixo transversal:
- `stretch` (padrão) 🔼🔽 os itens esticam para preencher o espaço.
- `flex-start` ⬆️ alinha os itens no topo.
- `flex-end` ⬇️ alinha os itens na base.
- `center` 🔘 centraliza os itens.
- `baseline` 📏 alinha os itens pela linha base do texto.

🔹 **Exemplo:**
```css
.container {
  display: flex;
  align-items: center;
}
```

### 5️⃣ `flex-wrap`
Define se os itens devem ou não quebrar para uma nova linha:
- `nowrap` (padrão) 🚫 impede a quebra de linha.
- `wrap` ✅ permite a quebra de linha.
- `wrap-reverse` 🔄 permite a quebra, mas na direção inversa.

🔹 **Exemplo:**
```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

### 6️⃣ `align-content`
Controla o espaçamento entre as linhas quando há quebra de linha (`flex-wrap: wrap;`):
- `flex-start` 🔼 agrupa as linhas no topo.
- `flex-end` 🔽 agrupa as linhas na base.
- `center` 🔘 centraliza as linhas.
- `space-between` ↔️ espaçamento igual entre as linhas.
- `space-around` 🔄 espaçamento ao redor das linhas.
- `stretch` 🔼🔽 as linhas se expandem para preencher o espaço.

🔹 **Exemplo:**
```css
.container {
  display: flex;
  flex-wrap: wrap;
  align-content: center;
}
```

## 🧩 Um Pouco Sobre Flex Items
Os **Flex Items** são os elementos filhos dentro do container flexível. Algumas propriedades básicas que podem ser aplicadas a eles incluem:

- `flex-grow` ➡️ define o quanto um item pode crescer.
- `flex-shrink` ⬅️ define o quanto um item pode encolher.
- `flex-basis` 📏 define o tamanho inicial do item.
- `order` 🔢 define a ordem dos itens.
- `align-self` 🔄 permite alinhar um item individualmente.

🔹 **Exemplo:**
```css
.item {
  flex-grow: 1;
}
```

## 🚀 Conclusão
O **Flex Container** é a base do Flexbox e define como os itens flexíveis serão organizados. Com essas propriedades, você já consegue criar layouts responsivos e alinhamentos incríveis! 🔥

Agora é hora de testar! 🎨👨‍💻

