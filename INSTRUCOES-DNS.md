# Instruções para Configurar DNS do GitHub Pages

## Após a propagação dos nameservers (pode levar até 24h):

### 1. Acesse o painel de DNS da Hostinger:
https://hpanel.hostinger.com/domain/alumicalc.com/dns?tab=dns_records

### 2. Clique em "Adicionar registro" ou botão similar

### 3. Adicione 4 registros A:

**Registro A #1:**
- Tipo: A
- Nome: @ (ou deixe vazio)
- Aponta para: 185.199.108.153
- TTL: 14400 (ou padrão)

**Registro A #2:**
- Tipo: A
- Nome: @
- Aponta para: 185.199.109.153
- TTL: 14400

**Registro A #3:**
- Tipo: A
- Nome: @
- Aponta para: 185.199.110.153
- TTL: 14400

**Registro A #4:**
- Tipo: A
- Nome: @
- Aponta para: 185.199.111.153
- TTL: 14400

### 4. Adicione 1 registro CNAME:

**Registro CNAME:**
- Tipo: CNAME
- Nome: www
- Aponta para: djalmirribeiro.github.io
- TTL: 14400

### 5. Remova registros antigos:
- Remova qualquer registro A ou CNAME que aponte para outros servidores

### 6. Aguarde propagação:
- Pode levar de 5 minutos a 48 horas
- Teste em: https://dnschecker.org

### 7. Volte ao GitHub Pages:
- Acesse: https://github.com/DjalmirRibeiro/alumicalc/settings/pages
- Clique em "Check again"
- Quando o DNS estiver correto, marque "Enforce HTTPS"

## Seu site estará disponível em:
- https://alumicalc.com
- https://www.alumicalc.com

---

**Repositório GitHub:** https://github.com/DjalmirRibeiro/alumicalc
**GitHub Pages:** https://djalmirribeiro.github.io/alumicalc/
