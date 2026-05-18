# 💊 Pharmix

> Aplicativo mobile de apoio à automedicação responsável, com foco na identificação de interações entre princípios ativos de medicamentos.

---

## 📋 Sobre o Projeto

A automedicação é uma prática amplamente disseminada no Brasil e, quando realizada sem orientação adequada, pode representar riscos sérios à saúde — especialmente pela combinação inadvertida de medicamentos incompatíveis. O **Pharmix** surge como uma ferramenta de apoio informacional, permitindo que o usuário verifique possíveis interações entre princípios ativos antes de utilizá-los simultaneamente.

O projeto se alinha à **ODS 3 da ONU – Saúde e Bem-Estar**, promovendo o uso mais seguro e consciente de medicamentos.

> ⚠️ O Pharmix **não substitui** a orientação de um profissional de saúde. A ferramenta é exclusivamente informacional e complementar ao acompanhamento médico e farmacêutico.

---

## ✨ Funcionalidades (MVP)

- 🔍 **Busca de princípios ativos** com campo de autocompletar
- ⚡ **Verificação de interações** entre dois ou mais princípios ativos selecionados
- 🚨 **Alertas visuais** com grau de severidade e descrição dos riscos
- 🕓 **Histórico de consultas** realizadas pelo usuário
- 📱 Compatível com **Android e iOS**

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologia |
|---|---|
| Linguagem | TypeScript |
| Framework mobile | React Native 0.81 + Expo SDK 54 |
| Estilização | NativeWind 4 (Tailwind CSS para RN) |
| Navegação | React Navigation 7 (stack + bottom tabs) |
| Animações | React Native Reanimated 4 + Gesture Handler |
| Ícones | Lucide React Native |
| Armazenamento local | AsyncStorage |
| Autocompletar | React Native Autocomplete Dropdown |
| API de dados | CRF-MG (`imses.crfmg.org.br`) |
| Design/Prototipação | Figma |
| Linting/Formatação | ESLint + Prettier (com plugin Tailwind) |
| Versionamento | Git + GitHub |

> **Nota sobre a API:** os dados de princípios ativos são consumidos da API disponibilizada pelo Conselho Regional de Farmácia de Minas Gerais (CRF-MG), cujo acesso foi viabilizado mediante contato direto com os desenvolvedores. Por limitações da API, as interações no MVP são verificadas por **princípios ativos**, não por nomes comerciais de medicamentos.

---

## 🗂️ Estrutura do Projeto

```
pharmix-front/
├── assets/          # Imagens e recursos estáticos
├── src/             # Código-fonte principal
├── App.tsx          # Componente raiz
├── index.ts         # Entry point
├── app.json         # Configurações do Expo
├── tailwind.config.js
└── package.json
```

---

## 🚀 Como Executar

### Pré-requisitos

- Node.js 18+
- Expo CLI (`npm install -g expo-cli`)
- Aplicativo **Expo Go** no celular (ou emulador Android/iOS)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/pharmix-ms/pharmix-front.git
cd pharmix-front

# Instale as dependências
npm install

# Inicie o projeto
npx expo start
```

Escaneie o QR Code com o Expo Go (Android) ou com a câmera (iOS).

---

## 🔭 Roadmap

O MVP atual é a primeira versão funcional do Pharmix. As próximas etapas planejadas incluem:

- [ ] **Backend próprio com Next.js** — substituindo a dependência da API externa e permitindo maior controle e escalabilidade dos dados farmacológicos
- [ ] **Integração de IA** — análise inteligente de interações medicamentosas, incluindo combinações não previamente cadastradas
- [ ] **Tela de Perfil Médico** — o usuário poderá informar condições como gravidez, alergias e doenças crônicas para receber alertas personalizados
- [ ] **Busca por nome comercial** — além dos princípios ativos, futuramente será possível pesquisar diretamente pelo nome do medicamento
- [ ] **Ampliação da base de dados** — cobertura de mais princípios ativos e combinações

---

## 👥 Equipe

Desenvolvido por estudantes da **Faculdade de Análise e Desenvolvimento de Sistemas – Senac Hub Academy**, Campo Grande – MS.

| Nome | Contato |
|---|---|
| Mateus Storti Hellmann | mateus54099606@aluno.ms.senac.br |
| Guilherme Nantes Bergamo | guilherme54098226@aluno.ms.senac.br |
| Maria Eduarda | maria54099376@aluno.ms.senac.br |

---

## 📄 Licença

Este projeto foi desenvolvido para fins acadêmicos.

---

<p align="center">Feito com ❤️ e TypeScript · Pharmix © 2026</p>
