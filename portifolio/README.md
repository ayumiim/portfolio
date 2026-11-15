# Portfólio Pessoal - Desenvolvimento de Sistemas

## Sobre o Projeto
Este projeto consiste em um portfólio pessoal responsivo desenvolvido como atividade prática da Agenda 15. O objetivo do site é apresentar meu perfil profissional, formação acadêmica, tecnologias que domino, projetos desenvolvidos ao longo do curso e canais diretos para contato.

## Tecnologias Utilizadas
* **HTML5:** Estruturação semântica das seções da página.
* **CSS3:** Estilização personalizada, controle de proporção de imagens, paleta de cores customizada e efeitos de transição.
* **Bootstrap 5.3.3:** Criação do layout responsivo (sistema de grids), barra de navegação (Navbar), carrossel de slides e cards.
* **Devicon:** Biblioteca de ícones para representação visual das tecnologias e ferramentas.
* **Git e GitHub Pages:** Versionamento de código e hospedagem gratuita do site estático.

## Funcionamento do Projeto
O site é estruturado em formato *One-Page* (página única) com navegação fluida:
1. **Menu de Navegação (Navbar):** Fixado no topo (`sticky-top`), adapta-se para dispositivos móveis com botão hambúrguer e direciona o usuário às seções internas via âncoras (`#perfil`, `#formacao`, `#projetos`, `#contato`).
2. **Área de Destaque (Carousel):** Apresenta slides rotativos com transição suave (`carousel-fade`).
3. **Perfil e Tecnologias:** Exibe foto, resumo profissional e cards organizados em colunas com as ferramentas estudadas.
4. **Formação e Projetos:** Apresenta a trajetória acadêmica e os trabalhos práticos em formato de cards alinhados.
5. **Contato e Rodapé:** Disponibiliza botões de ação rápida para e-mail e GitHub.

## Recursos Novos Adicionados
Para evoluir o modelo apresentado em aula, foram implementados três recursos principais:
1. **Personalização da Identidade Visual (Paleta de Cores):** Substituição das classes padrão azuis do Bootstrap (`primary`) por uma paleta de cores personalizada nos títulos, badges e botões.
2. **Animações e Transições Interativas (`hover`):** Efeito visual de elevação e destaque de sombra ao passar o cursor sobre os cards, além de rolagem suave (`scroll-behavior: smooth`) na navegação.
3. **Nova Seção de Formação e Qualificações:** Adição de uma seção dedicada exclusivamente à formação técnica na ETEC e cursos complementares, integrada ao menu principal.

## Como os Recursos Foram Implementados
* **Identidade Visual:** Utilização de estilização inline (`style="color: ..."` e `style="background-color: ..."`) nos títulos, badges e botões de ação para definir uma paleta harmônica em todas as seções.
* **Animações CSS:** Criação da classe personalizada `.card-animado` dentro da tag `<style>` no `<head>`, utilizando `transition: transform 0.3s ease, box-shadow 0.3s ease` e a pseudoclasse `:hover` com `transform: translateY(-8px)`.
* **Seção de Formação:** Criação de uma nova `<section id="formacao">` utilizando o sistema de grid do Bootstrap (`container`, `row` e `col-md-6`) com componentes `card` e `badge`, vinculada a um novo item na Navbar.