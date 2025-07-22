# 🤖 Meu Copiloto Personalizado – Microsoft Copilot Studio

Este repositório documenta o processo de criação de um Copiloto personalizado utilizando o **Microsoft Copilot Studio**, incluindo passos, configurações e dicas para integração com Microsoft 365.

---

## 🧠 Objetivo

Criar um Copiloto que responde dúvidas frequentes de colaboradores sobre **controle de ponto eletrônico**, como horários de entrada/saída, banco de horas e justificativas.

---

## 🚀 Etapas de Criação

### 1. Acesse o Copilot Studio

- URL: [https://copilotstudio.microsoft.com](https://copilotstudio.microsoft.com)
- Faça login com sua conta corporativa que tenha **permissão para criar copilotos**.

---

### 2. Criar um novo Copiloto

1. Clique em **"Criar copilot"**
2. Dê um nome, por exemplo: `Copiloto RH - Controle de Ponto`
3. Escolha o idioma (ex: Português - Brasil)
4. Opcional: selecione um modelo (template) existente

---

### 3. Defina os Tópicos

Crie tópicos com base nas perguntas mais frequentes:

| Nome do Tópico           | Frases de Gatilho                                      | Resposta Base                                                                 |
|--------------------------|--------------------------------------------------------|-------------------------------------------------------------------------------|
| Horário de Entrada       | "Qual meu horário?", "Que horas entro?"               | "Seu horário padrão é das 8h às 17h com 1h de almoço."                        |
| Justificativa de Atraso | "Como justifico atraso?", "Fiquei preso no trânsito"   | "Acesse o sistema de ponto e selecione a opção 'Justificativa'."             |
| Banco de Horas           | "Quantas horas extras tenho?", "Banco de horas"       | "Você pode consultar seu saldo de horas no portal de RH."                    |

---

### 4. Conecte com Fontes Externas (opcional)

Você pode adicionar:

- Documentos internos (PDF, Word, etc.)
- URLs do SharePoint ou Teams
- Conectores como Power Automate para interagir com sistemas

---

### 5. Publique o Copiloto

1. Vá para **Publicar > Publicar agora**
2. Escolha os canais de publicação:
   - Microsoft Teams
   - Website (via iframe)
   - Power Apps

---

## 🌐 Exemplo de Embed em Website

Você pode embutir o copiloto num site com o seguinte iframe:

```html
<iframe
  src="https://copilotstudio.microsoft.com/embed/YOUR_COPILOT_ID"
  width="400"
  height="600"
  frameborder="0"
></iframe>
