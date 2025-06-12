QRio

Um aplicativo web moderno e fácil de usar para gerar e ler códigos QR. Crie QRs para texto, URLs, e-mails, telefones e redes WiFi, ou escaneie QRs usando a câmera do dispositivo ou imagens carregadas. Desenvolvido com HTML, CSS (Tailwind CSS), e JavaScript, com suporte a temas claro/escuro e interface responsiva.
Funcionalidades

Geração de QR Code:
Suporta múltiplos tipos de conteúdo: Texto, URL, E-mail, Telefone e WiFi.
Validação de entrada para URLs e e-mails.
Download do QR Code como PNG.
Cópia da imagem do QR Code para a área de transferência.


Leitura de QR Code:
Escaneamento em tempo real usando a câmera do dispositivo.
Leitura de QRs a partir de imagens carregadas (máximo 5MB).
Suporte a arrastar e soltar para upload de imagens.
Cópia do conteúdo escaneado para a área de transferência.


Interface de Usuário:
Design responsivo para desktop e dispositivos móveis.
Alternância entre temas claro e escuro com persistência via localStorage.
Animações suaves e efeitos visuais (ex.: glassmorphism, elementos flutuantes).
Atalhos de teclado (ex.: Ctrl+G para gerar, Ctrl+R para ler).


SEO e Acessibilidade:
Tags meta otimizadas para motores de busca e redes sociais (Open Graph, Twitter Cards).
Atributos aria-label para acessibilidade.
Favicon para navegadores e dispositivos móveis.


Desempenho:
Código JavaScript modularizado e minificável.
Uso de bibliotecas leves como qrcodejs e qr-scanner.



Tecnologias Utilizadas

Frontend:
HTML5
CSS (Tailwind CSS para estilização)
JavaScript (ES Modules)


Bibliotecas:
qrcodejs para geração de QR Codes.
qr-scanner para leitura de QR Codes.


Outros:
Favicon para branding.
Tags meta para SEO e compartilhamento em redes sociais.



Estrutura do Projeto
project/
├── assets/
│   ├── css/
│   │   └── style.css        # Estilos personalizados
│   ├── images/
│   │   ├── favicon.ico      # Favicon para navegadores
│   │   ├── favicon-512x512.png # Ícone para dispositivos móveis
│   │   └── og-image.jpg     # Imagem para Open Graph/Twitter Cards
│   ├── js/
│   │   ├── script.js        # Lógica principal (ou script.min.js se minificado)
│   │   ├── qr-scanner.min.js # Biblioteca para leitura de QR Codes
│   │   └── qr-scanner.worker.min.js # Worker para qr-scanner
├── index.html               # Página principal
└── README.md                # Documentação do projeto

Instalação

Clone o repositório:
git clone https://github.com/seu-usuario/qr-code-generator-reader.git
cd qr-code-generator-reader


Hospede em um servidor local:Como o projeto usa módulos JavaScript (type="module"), você precisa de um servidor para evitar erros de CORS. Use uma das opções abaixo:

Live Server (extensão do VS Code).
Node.js http-server:npm install -g http-server
http-server .


Abra o navegador em http://localhost:8080.


Dependências externas:

O projeto usa CDNs para qrcodejs e Tailwind CSS, então não é necessário instalar dependências adicionais, desde que os arquivos qr-scanner.min.js e qr-scanner.worker.min.js estejam em assets/js.



Uso

Gerar QR Code:

Acesse a aba "Gerar QR Code".
Selecione o tipo de conteúdo (Texto, URL, E-mail, Telefone ou WiFi).
Preencha os campos correspondentes.
Clique em "Gerar QR Code".
Baixe o QR como PNG ou copie a imagem para a área de transferência.


Ler QR Code:

Acesse a aba "Ler QR Code".
Clique em "Iniciar Câmera" para escanear com a câmera ou arraste uma imagem para o campo de upload.
O resultado será exibido e pode ser copiado.


Alternar Tema:

Use o toggle no canto superior direito para alternar entre os temas claro e escuro.


Atalhos de Teclado:

Ctrl+G: Abre a aba de geração.
Ctrl+R: Abre a aba de leitura.
Ctrl+Enter: Gera o QR Code (na aba de geração).



Contribuição

Fork o repositório.
Crie uma branch para sua feature:git checkout -b minha-feature


Commit suas alterações:git commit -m "Adiciona minha feature"


Push para o repositório remoto:git push origin minha-feature


Abra um Pull Request.

Licença
Este projeto está licenciado sob a MIT License.
Contato

Autor: Seu Nome ou Nome da Empresa
Email: seu-email@exemplo.com
GitHub: seu-usuario


Agradecimentos:

Às bibliotecas qrcodejs e qr-scanner por possibilitarem as funcionalidades principais.
Ao Tailwind CSS por facilitar a estilização.

