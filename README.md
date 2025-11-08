
📄 README para index.html (MF Seguros - Cotação de Planos de Saúde)
Este arquivo HTML é a página inicial (landing page) da MF Seguros, uma corretora especializada em cotação de planos de saúde no Rio de Janeiro. A página tem como objetivo principal gerar leads por meio de um formulário de cotação rápida via WhatsApp.

🚀 Visão Geral e Estrutura
O design da página é responsivo e utiliza o Tailwind CSS para estilização. O layout é focado em uma seção de herói de alto impacto com um vídeo de fundo e um formulário de cotação de destaque.

🎨 Tecnologias Utilizadas
HTML5

CSS Puro (para estilos específicos como o fundo de vídeo e animações)

Tailwind CSS (via CDN, com configuração customizada de cores)

JavaScript (para o formulário de WhatsApp e controle de áudio do vídeo)

Google Fonts (Inter)

⚙️ Cores Customizadas (Tailwind Config)
A página utiliza uma paleta de cores institucional definida no bloco <script> do Tailwind:

mf-blue: #1a3765 (Azul principal, dominante no rodapé e textos)

mf-light-blue: #2a6a9b (Azul claro de acento)

mf-accent: #25D366 (Verde do WhatsApp, usado para botões de CTA e animação)

🧱 Principais Seções
1. Cabeçalho (<header>)
Conteúdo: Logo da MF Seguros e um botão "Fale Agora" fixo para contato direto via WhatsApp.

Funcionalidade: Fixo (fixed) e com alto z-index para estar sempre visível.

2. Seção Hero (<section class="hero">)
Vídeo de Fundo: Um vídeo em loop (video/Aug_19__2133_29s_202508192223_bo4k4.mp4) é usado como plano de fundo, com um filtro brightness(40%) aplicado via CSS para melhorar a legibilidade.

Controle de Áudio: Um botão (#audioButton) permite ao usuário silenciar/ativar o áudio do vídeo.

Título Principal (H1): "Sua Saúde Não Espera."

Call to Action (CTA): O formulário de "Cotação Rápida em 1 Minuto!" é o ponto focal.

3. Formulário de Cotação (#whatsappForm)
Campos: Nome Completo e Telefone (DDD + Número).

Validação: O campo de telefone exige o padrão [0-9]{10,11} (10 ou 11 dígitos, como 21987654321).

Envio (JavaScript): Ao enviar, o script monta uma mensagem pré-preenchida com o nome e telefone do usuário e abre uma nova aba/janela do WhatsApp Web/App para o número 5521987681403.

4. Operadoras (#operadoras)
Conteúdo: Lista as principais operadoras de planos de saúde parceiras, incluindo Bradesco Saúde, SulAmérica Saúde, Porto Seguro Saúde, e MedSênior.

Estilo: Utiliza um layout de grid e inclui um efeito de hover para as caixas das operadoras (hover:scale-105).

5. Rodapé (<footer>)
Conteúdo: Informações de copyright (© 2025) e o telefone de contato via WhatsApp.

6. Botão Flutuante (WhatsApp)
Funcionalidade: Botão de WhatsApp fixo no canto inferior direito.

Animação: Possui a animação CSS @keyframes pulse-whatsapp para chamar a atenção do usuário.

💻 Scripts de Funcionalidade
O arquivo contém um bloco <script> no final do <body> para duas funcionalidades principais:

Manipulação do Formulário (whatsappForm):

Captura os valores de Nome e Telefone.

Codifica a mensagem.

Redireciona para o WhatsApp com a mensagem pré-preenchida.

Exibe uma mensagem de erro no botão de submit se os campos estiverem vazios.

Controle de Áudio do Vídeo (audioButton):

Alterna o estado muted do elemento <video> (#bgVideo).

Atualiza o texto do botão para "🔈 Ativar Áudio" ou "🔇 Silenciar Áudio" conforme o estado.

📸 Imagens e Vídeos Necessários
A página depende da existência dos seguintes arquivos de mídia para ser renderizada corretamente:

img/LOGO.PNG

img/bradesco.jpg

img/sulamerica.jpg

img/porto.jpg

img/medsenior.jpg

video/Aug_19__2133_29s_202508192223_bo4k4.mp4

⚠️ Observações de Desenvolvimento
O Tailwind CSS está sendo carregado via CDN, o que é rápido para prototipagem/páginas simples, mas pode não ser ideal para produção em grande escala.

O número de WhatsApp de contato utilizado em todos os links e formulários é (21) 98768-1403 (5521987681403).
