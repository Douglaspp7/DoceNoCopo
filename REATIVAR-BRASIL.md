# 🇧🇷 Checklist de Reativação — Lançamento Brasil

> Estado atual (fase só-espanhol): tráfego 100% ES. O lado BR está **pronto e pausado**.
> Quando for abrir o Brasil, siga esta lista na ordem. Cada item diz exatamente o que mexer.

---

## 1. App (repo `DulceVaso_app`)
**Reativar o seletor de idioma 🇧🇷/🇪🇸**
- Arquivo: `index.html` (≈ linha 29, comentário "Seletor de idioma")
- Trocar `display:none` → `display:flex` no `<div>` do seletor
- As traduções PT já estão no `i18n.js` (intactas) — não precisa mexer em mais nada
- Commit + deploy (merge na `main`)

---

## 2. Landing BR (repo `DoceNoCopo` → doce-no-copo.pages.dev)
- ✅ Já está **no ar e pronta** (preço R$ 37, ROI, depoimentos, marca consistente)
- Confirmar que o preço da página **bate com a Hotmart** (R$ 37)
- **Recomendado:** replicar na BR as melhorias que vencerem no teste ES
  (ex.: prova social no terço superior, imagens otimizadas) — só depois de validadas no ES

---

## 3. Hotmart (produto BR `M106366783X`)
- [ ] Pixel `1329933185770980` + evento **Purchase** + **API de Conversões (token)** linkados ao produto BR
- [ ] Preço **R$ 37,00**
- [ ] **Order bump** anexado: `Order Pump/manual_substituicoes_pt_embutido.html` → gerar PDF (Imprimir → Salvar como PDF, "Gráficos de plano de fundo" ligado)
- [ ] (Futuro) **Upsell pós-compra** configurado
- [ ] **Recuperação de carrinho abandonado** ativada

---

## 4. Meta Ads
- [ ] **Reativar (despausar) o conjunto Português**
- [ ] Confirmar que os anúncios BR apontam para **doce-no-copo** → checkout **R$** (`M106366783X`)
- [ ] Evento de otimização: **InitiateCheckout** no começo (pouco volume) → migrar para **Compra** só quando tiver ~30–50 vendas/semana (criar campanha NOVA, não editar a de IC)
- [ ] Investigar por que o BR sub-entregou antes (público pequeno / orçamento / CPM):
      considerar **público mais amplo** ou **orçamento maior** no conjunto BR
- [ ] Reforçar criativos BR (o "Criativo 1 Português" tinha CTR fraco de 3,69%)

---

## 5. Rastreamento / Conversões Personalizadas (BR)
Criar no Gerenciador de Eventos, **sempre com regra URL contém `doce-no-copo`**:
- [ ] `Viu_Depoimentos` BR
- [ ] `Viu_Preco` BR
- [ ] `Scroll_50` BR

Funil a ler: **ViewContent → Viu_Depoimentos → Viu_Preco → InitiateCheckout → Purchase**

---

## 6. Verificação final (go-live)
- [ ] Compra-teste BR em aba anônima → mostra **R$ 37**, **PIX gera QR Code**, compra conclui
- [ ] Confirmar no Gerenciador de Eventos que o **Purchase** disparou (origem Servidor/CAPI)
- [ ] **Estornar** a compra-teste
- [ ] Soltar orçamento e acompanhar o funil pelos 4 números acima

---

### Referência rápida de códigos
| Item | Valor |
|---|---|
| Pixel | `1329933185770980` |
| Checkout BR | `M106366783X` (R$) |
| Checkout ES | `I106284787G` (USD) |
| Landing BR | doce-no-copo.pages.dev |
| Landing ES | douglaspp7.github.io/DulceVaso |
