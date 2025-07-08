# Igreja Evangélica Nova Jerusalém - Site Institucional

![IENJ Logo](https://img.shields.io/badge/IENJ-Igreja%20Nova%20Jerusalém-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 📋 Visão Geral do Projeto

Este é o site institucional da **Igreja Evangélica Nova Jerusalém**, uma comunidade de fé localizada em Recife, PE. O site foi desenvolvido com foco na acessibilidade, responsividade e experiência do usuário, utilizando apenas tecnologias web nativas (HTML, CSS e JavaScript puro).

### 🎯 Objetivos

- Apresentar a igreja e sua missão à comunidade
- Facilitar o contato e a comunicação com os membros
- Divulgar eventos, cultos e projetos sociais
- Oferecer informações sobre localização e horários
- Disponibilizar canal para doações e contribuições
- Compartilhar conteúdo através do blog/notícias

## 🛠 Tecnologias Utilizadas

### Frontend
- **HTML5** - Estrutura semântica e acessível
- **CSS3** - Estilização moderna com CSS Grid, Flexbox e CSS Custom Properties
- **JavaScript ES6+** - Interatividade e funcionalidades dinâmicas

### Bibliotecas e Recursos Externos
- **Google Fonts** (Inter) - Tipografia moderna
- **Font Awesome 6** - Ícones
- **Google Maps Embed API** - Mapa de localização
- **Unsplash** - Imagens de exemplo (substitua por imagens reais)

### Características Técnicas
- **Design Responsivo** (Mobile-First)
- **Acessibilidade Web** (WCAG 2.1 Guidelines)
- **SEO Otimizado** (Meta tags, Schema markup ready)
- **Performance Otimizada** (Lazy loading, otimização de imagens)
- **Cross-browser Compatible**

## 📁 Estrutura de Pastas

```
ienjrecife/
│
├── index.html              # Página principal
├── README.md              # Este arquivo
│
├── css/
│   └── styles.css         # Folha de estilos principal
│
└── js/
    └── script.js          # Scripts JavaScript
```

### 📄 Estrutura do Site

O site está organizado nas seguintes seções:

1. **Header/Navegação** - Menu responsivo com links para todas as seções
2. **Home** - Seção de boas-vindas com call-to-action
3. **Sobre Nós** - História da igreja, valores e missão
4. **Nossa Missão** - Visão, propósito e foco de atuação
5. **Equipe Pastoral** - Apresentação dos líderes com fotos e biografias
6. **Cultos e Eventos** - Horários dos cultos e calendário de eventos
7. **Projetos Sociais** - Ações comunitárias e oportunidades de voluntariado
8. **Galeria** - Fotos de encontros, celebrações e ações (com filtros)
9. **Blog/Notícias** - Artigos, mensagens e atualizações
10. **Contato** - Formulário de contato e informações
11. **Localização** - Mapa integrado e informações de acesso
12. **Doações** - Informações para contribuições financeiras
13. **Footer** - Links úteis, contato e redes sociais

## 🚀 Como Executar Localmente

### Pré-requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Servidor web local (opcional, mas recomendado)

### Opção 1: Abrir Diretamente no Navegador
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/ienjrecife.git

# Navegue até a pasta
cd ienjrecife

# Abra o arquivo index.html no seu navegador
# Duplo clique no arquivo ou arraste para o navegador
```

### Opção 2: Usando um Servidor Local

#### Com Python (se instalado):
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Acesse: http://localhost:8000
```

#### Com Node.js (se instalado):
```bash
# Instale um servidor simples globalmente
npm install -g http-server

# Execute no diretório do projeto
http-server

# Acesse: http://localhost:8080
```

#### Com PHP (se instalado):
```bash
php -S localhost:8000
```

#### Com VS Code:
- Instale a extensão "Live Server"
- Clique com o botão direito em `index.html`
- Selecione "Open with Live Server"

## 🎨 Personalização

### 🎨 Cores e Tema

As cores principais estão definidas como CSS Custom Properties no arquivo `css/styles.css`:

```css
:root {
    --primary-color: #2563eb;        /* Azul principal */
    --primary-dark: #1d4ed8;         /* Azul escuro */
    --secondary-color: #f59e0b;      /* Amarelo/Laranja */
    --dark-color: #1f2937;           /* Texto escuro */
    --light-color: #f8fafc;          /* Fundo claro */
    /* ... outras variáveis */
}
```

Para personalizar as cores:
1. Abra `css/styles.css`
2. Modifique os valores das variáveis CSS
3. As mudanças serão aplicadas automaticamente em todo o site

### 📝 Conteúdo

#### Textos e Informações
- **Títulos e descrições**: Edite diretamente no arquivo `index.html`
- **Informações de contato**: Atualize na seção `#contato`
- **Dados da equipe pastoral**: Modifique na seção `#equipe`
- **Horários de cultos**: Atualize na seção `#cultos`

#### Imagens
1. Substitua as URLs do Unsplash por imagens reais da igreja
2. Coloque as imagens em uma pasta `images/` ou `assets/`
3. Atualize os caminhos no HTML
4. Mantenha o atributo `alt` para acessibilidade

#### Exemplo de substituição de imagem:
```html
<!-- Antes -->
<img src="https://images.unsplash.com/photo-..." alt="Descrição">

<!-- Depois -->
<img src="images/igreja-fachada.jpg" alt="Fachada da Igreja Nova Jerusalém">
```

### 🌍 Google Maps

Para atualizar a localização no mapa:
1. Acesse o [Google Maps](https://maps.google.com)
2. Encontre a localização da igreja
3. Clique em "Compartilhar" > "Incorporar um mapa"
4. Copie o código HTML
5. Substitua o iframe na seção `#localizacao`

### 📧 Formulário de Contato

O formulário atualmente simula o envio. Para implementar o envio real:

1. **Backend necessário**: Configure um servidor (PHP, Node.js, Python, etc.)
2. **Substitua a função `submitForm()`** em `js/script.js`
3. **Exemplo com fetch API**:

```javascript
function submitForm(data) {
    fetch('/enviar-contato.php', {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
        },
        body: JSON.stringify(data)
    })
    .then(response => response.json())
    .then(result => {
        if (result.success) {
            showNotification('Mensagem enviada com sucesso!', 'success');
        } else {
            showNotification('Erro ao enviar mensagem.', 'error');
        }
    });
}
```

## 🌐 Deploy (Publicação)

### Opções de Hospedagem Gratuita

#### 1. GitHub Pages
```bash
# Faça push do código para o GitHub
git add .
git commit -m "Site da igreja"
git push origin main

# Ative o GitHub Pages nas configurações do repositório
# Acesse: https://seu-usuario.github.io/ienjrecife
```

#### 2. Netlify
1. Faça upload da pasta do projeto em [netlify.com](https://netlify.com)
2. Ou conecte seu repositório GitHub
3. O site será publicado automaticamente

#### 3. Vercel
1. Conecte seu repositório em [vercel.com](https://vercel.com)
2. Deploy automático a cada push

#### 4. Surge.sh
```bash
npm install -g surge
surge
# Siga as instruções
```

### Hospedagem Paga
- **Hostinger**, **Hostgator**, **SiteGround**
- **AWS S3 + CloudFront**
- **Google Cloud Storage**

## 📱 Funcionalidades Implementadas

### ✅ Navegação
- [x] Menu responsivo com hamburger para mobile
- [x] Navegação suave entre seções
- [x] Highlight do link ativo baseado no scroll
- [x] Header com efeito de transparência no scroll

### ✅ Formulários
- [x] Validação completa do formulário de contato
- [x] Mensagens de erro personalizadas
- [x] Estados de loading e sucesso
- [x] Notificações toast

### ✅ Galeria
- [x] Sistema de filtros por categoria
- [x] Modal/lightbox para visualização de imagens
- [x] Animações suaves de transição

### ✅ Interatividade
- [x] Animações de entrada dos elementos
- [x] Contadores animados para estatísticas
- [x] Botão "voltar ao topo"
- [x] Lazy loading de imagens

### ✅ Acessibilidade
- [x] Navegação por teclado
- [x] Labels adequados nos formulários
- [x] Contraste de cores adequado
- [x] Textos alternativos em imagens
- [x] Estrutura semântica HTML5

### ✅ Performance
- [x] CSS e JS otimizados
- [x] Carregamento assíncrono de recursos
- [x] Compressão de imagens (quando implementado)

## 📋 Próximos Passos (Opcional)

### 🔄 Melhorias Futuras
- [ ] Sistema de CMS para edição de conteúdo
- [ ] Blog dinâmico com backend
- [ ] Sistema de newsletter
- [ ] Integração com redes sociais
- [ ] PWA (Progressive Web App)
- [ ] Modo escuro/claro
- [ ] Múltiplos idiomas
- [ ] Chat online
- [ ] Sistema de agendamento de visitas

### 🔧 Tecnologias para Evolução
- **Backend**: Node.js, PHP, Python (Django/Flask)
- **CMS**: WordPress, Strapi, Sanity
- **Database**: MySQL, PostgreSQL, MongoDB
- **Autenticação**: Firebase Auth, Auth0

## 📞 Informações de Contato da Igreja

> **Importante**: Atualize estas informações com os dados reais da igreja

- **Endereço**: Rua da Esperança, 123 - Boa Viagem, Recife - PE
- **CEP**: 51021-040
- **Telefone**: (81) 3456-7890
- **WhatsApp**: (81) 99999-8888
- **E-mail**: contato@ienjrecife.com.br
- **Site**: www.ienjrecife.com.br

### Horários de Funcionamento
- **Segunda a Sexta**: 8h às 17h
- **Sábado**: 8h às 12h  
- **Domingo**: 7h às 21h

### Horários de Cultos
- **Domingo**: 9h e 19h
- **Quarta-feira** (Oração): 19h30
- **Sexta-feira** (Jovens): 19h30
- **Escola Dominical**: 8h

## 🤝 Contribuições

Se você quiser contribuir com melhorias para o site:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## 📄 Licença

Este projeto foi desenvolvido especificamente para a Igreja Evangélica Nova Jerusalém. Para uso em outras organizações religiosas, entre em contato para autorização.

## 💡 Suporte Técnico

Para dúvidas técnicas sobre o site:

- **Desenvolvedor**: [Seu Nome]
- **E-mail**: [seu.email@exemplo.com]
- **GitHub**: [seu-usuario]

---

*"Porque onde estiverem dois ou três reunidos em meu nome, aí estou eu no meio deles." - Mateus 18:20*

**Desenvolvido com ❤️ para a glória de Deus**
