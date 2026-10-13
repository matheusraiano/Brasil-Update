# Brazil Update+ v5.2 - Revolta da Vacina e Zona da Mata

## 🎭 Novo Evento Histórico

### Revolta da Vacina (1904)

Evento único sobre a revolta popular no Rio de Janeiro contra a vacinação obrigatória durante a modernização urbana.

**Trigger:**
- Brasil entre 1904-1920
- Rio de Janeiro como capital
- Urbanização mínima (5+ níveis de urban center)
- Tecnologia de prevenção de malária
- Não estar em guerra

**3 Opções Balanceadas:**

1. **Reprimir com força militar**
   - +25 autoridade, +5 aprovação latifundiários
   - -15 aprovação pequena burguesia
   - Radicalização massiva no Rio (24 meses)

2. **Negociar e amenizar campanha**
   - -5% mortalidade gradual
   - +5% qualificação populacional
   - Menos resistência (36 meses)

3. **Educação popular** (custa £50,000, requer Academia)
   - -10% mortalidade
   - +10% legitimidade
   - +15% eficiência hospitais
   - Bonus de educação em saúde (60 meses)
   - Melhor opção de longo prazo!

## 🌿 Nova Trait Geográfica

### Zona da Mata

Faixa litorânea úmida do Nordeste brasileiro, caracterizada por clima tropical úmido e solo fértil.

**Efeitos:**
- +20% throughput plantações de açúcar
- +15% throughput plantações de café
- +10% throughput plantações de tabaco
- +15 terra arável
- +10% throughput plantations (geral)
- +5% atração de migração

**Aplicada em:**
- Pernambuco
- Alagoas
- Sergipe
- Paraíba

Esta trait diferencia o litoral úmido do sertão seco interior, refletindo a realidade geográfica e econômica da região.

## 💎 Novos Recursos Naturais

### Manganês em Amapá
- **+30 ferro não descoberto**
- Representa os depósitos de Serra do Navio
- Descoberta tardia mas estratégica para indústria

### Cassiterita em Rondônia
- **+15 chumbo (capped resource)**
- Representa estanho (cassiterita) histórico da região
- Importante para indústria e tecnologia

## 🔧 Correções Críticas

### Bug do Brasil Branco (Critical Fix)
**Problema:** Erro de sintaxe no arquivo de Amapá causava todo o Brasil aparecer branco/sem dono no mapa
**Causa:** Faltava `resource = {` antes da definição de gold_field
**Status:** ✅ CORRIGIDO

### Bug de Alagoas (Critical Fix)
**Problema:** Estado de Alagoas não carregava traits nem aparecia corretamente
**Causa:** Faltava aspas de fechamento em province ID (`"xA08050 "` → `"xA08050"`)
**Status:** ✅ CORRIGIDO

### Ícone da Trait
**Problema:** Zona da Mata usava `forest.dds` que não existe
**Solução:** Mudado para `good_soils.dds` (usado por Terra Roxa e outras)
**Status:** ✅ CORRIGIDO

## 📊 Estatísticas v5.2

- **1 evento novo** (Revolta da Vacina)
- **4 modificadores novos** (saúde pública)
- **1 trait nova** (Zona da Mata)
- **2 recursos adicionados** (Manganês, Cassiterita)
- **3 bugs críticos corrigidos**
- **100% localizado** em PT-BR

## 📦 Instalação

1. Baixe o arquivo `.zip` abaixo
2. Extraia para `Documents/Paradox Interactive/Victoria 3/mod/`
3. Ative o mod no launcher do jogo

**Ou atualize da v5.1:**
- Substitua a pasta antiga pela nova
- Save games compatíveis (novos eventos aparecem gradualmente)

## 🎮 Como Testar

### Revolta da Vacina
1. Jogue como Brasil
2. Mantenha Rio de Janeiro como capital
3. Desenvolva urbanização no Rio (5+ urban center)
4. Pesquise "Malaria Prevention"
5. Avance até 1904
6. O evento deve aparecer!

### Zona da Mata
1. Abra estados nordestinos: PE, AL, SE, PB
2. Verifique trait "Zona da Mata" com ícone de solos bons
3. Observe bonus em plantações de açúcar/café

### Recursos
- Amapá: Minerar ferro (Serra do Navio)
- Rondônia: Extrair chumbo (cassiterita)

## ⚠️ Compatibilidade

- ✅ Victoria 3 versão 1.0+
- ✅ Compatível com v5.1 (atualização incremental)
- ✅ Compatível com save games
- ✅ Funciona com ou sem DLC "Colossus of the South"
- ⚠️ Pode conflitar com mods que modificam mapa da América do Sul

## 🆕 Arquivos Novos

```
events/brazil_vaccine_revolt.txt
localization/braz_por/events/brazil_vaccine_revolt_l_braz_por.yml
ANALISE_VANILLA_VS_MOD.md
PROGRESSO_V5.2.md
```

## 📝 Arquivos Modificados

```
common/modifiers/00_brazil_update_modifiers.txt (+4 modificadores)
common/state_traits/00_brazil_traits.txt (+1 trait)
map_data/state_regions/07_south_america.txt (correções + trait + recursos)
localization/braz_por/map/traits_l_braz_por.yml (+1 localização)
CHANGELOG.md (atualizado)
```

## 🐛 Bugs Conhecidos

Nenhum conhecido até o momento. Todos os bugs da v5.1 foram corrigidos!

## 📜 Changelog Completo

### Adicionado
- Revolta da Vacina (1904) - evento histórico único
- Trait Zona da Mata - faixa litorânea nordestina
- Manganês em Amapá (+30 ferro)
- Cassiterita em Rondônia (+15 chumbo)
- 4 modificadores de saúde pública

### Corrigido
- Bug crítico que causava Brasil branco (sintaxe Amapá)
- Bug crítico de Alagoas (aspas faltando)
- Ícone da trait Zona da Mata

### Alterado
- Aplicada Zona da Mata em 4 estados nordestinos

## 🚀 Próxima Versão (v5.3)

Em planejamento:
- Guerra do Paraguai expandida (eventos de batalhas)
- Journal Entry do Ciclo do Café
- Mais eventos regionais
- Flavor text PT-BR para estados

---

**Desenvolvido por**: metelrzx  
**Licença**: MIT  
**GitHub**: https://github.com/matheusraiano/Brasil-Update

**Agradecimentos especiais à comunidade brasileira de Victoria 3!** 🇧🇷
