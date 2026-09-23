# Landing Page de Redirecionamento para WhatsApp (BitSAC)

Landing page inspirada no padrão da [Apex Inteligência Comercial](https://apexinteligenciacomercial.com.br/obrigado), otimizada para alta conversão e redirecionamento para o WhatsApp com as cores e identidade visual da **BitSAC** (Meta Business Partner).

---

## 📱 Dados Configurados

- **Número de WhatsApp:** `(44) 9136-7439` (configurado como `554491367439`)
- **Mensagem Pré-configurada:**
  > *"Preenchi o formulário de vocês e gostaria do diagnóstico de atendimento!"*
- **Link Direto Gerado:**
  `https://wa.me/554491367439?text=Preenchi%20o%20formul%C3%A1rio%20de%20voc%C3%AAs%20e%20gostaria%20do%20diagn%C3%B3stico%20de%20atendimento%21`

---

## 🎨 Destaques do Design

1. **Identidade Visual BitSAC & Meta Partner:**
   - Paleta escura estilo OLED / Midnight (`#070D15`) com glows radiais em **Turquesa / Teal BitSAC (`#00D2B4`)** e **Verde WhatsApp (`#25D366`)**.
   - Logo SVG vetorial nítido da BitSAC com balão de conversa e selo oficial **Meta Business Partner**.
   - Tipografia moderna e legível (*Plus Jakarta Sans*, *Space Grotesk* e *JetBrains Mono*).

2. **Dores do Criativo / Diagnóstico de Atendimento:**
   - Cards destacando as soluções para as dores do anúncio:
     - 🕒 *Fim da fila de espera (atendimento sem 1 hora de espera)*
     - 💬 *Histórico centralizado (sem repetir a mesma informação)*
     - 📱 *Integração Omnichannel (WhatsApp, Instagram e Facebook unificados)*

3. **Card de Ação (Double-Bezel):**
   - Mockup realista de balão do WhatsApp com a mensagem pré-digitada e checks azuis de confirmação.
   - Botão CTA pulsante de alta conversão.
   - Barra de contagem regressiva de 5 segundos com botão de pausar/retomar.

4. **Pronto para Tráfego Pago & Rastreamento:**
   - Estrutura pronta para **Meta Pixel (`fbq`)** com eventos automáticos de `PageView`, `Lead` e `Contact`.
   - Compatível com Google Tag Manager / GA4.
   - Preservação e repasse inteligente de parâmetros UTM.

---

## ⚙️ Como Personalizar

No arquivo `index.html`, localize o bloco de script no final da página:

```javascript
const PHONE_NUMBER = "554491367439"; // Altere para 5544991367439 se necessário
const MESSAGE = "Preenchi o formulário de vocês e gostaria do diagnóstico de atendimento!";
```

### Configurar seu Meta Pixel ID
No `<head>` do `index.html`, descomente e insira o seu ID:
```javascript
fbq('init', 'SEU_PIXEL_ID_AQUI');
fbq('track', 'PageView');
fbq('track', 'Lead');
```

---

## 🚀 Como Visualizar e Hospedar

Você pode abrir o arquivo `index.html` diretamente no seu navegador, ou rodar um servidor local rápido:

```bash
# Na pasta do projeto:
python3 -m http.server 3000
```
Depois acesse: `http://localhost:3000`

Pode ser hospedado gratuitamente em qualquer serviço estático como Vercel, Netlify, Cloudflare Pages, GitHub Pages ou em qualquer hospedagem cPanel/WordPress.
