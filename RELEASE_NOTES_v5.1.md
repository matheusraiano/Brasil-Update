# Brazil Update+ v5.1 - Novas Culturas e Sistema de Integração Nacional

## 🎭 3 Novas Culturas Brasileiras

Esta versão adiciona diversidade cultural ao Brasil com 3 novas culturas regionais, cada uma com identidade própria:

- **Mineiro** (Minas Gerais) - Cultura da mineração e barroco colonial, obsessão: ouro
- **Carioca** (Rio de Janeiro) - Elite cosmopolita da capital imperial, obsessão: móveis de luxo  
- **Sertanejo** (Centro-Oeste) - Cultura do interior adaptada ao cerrado, obsessão: tecidos

Cada cultura tem nomes próprios, sobrenomes históricos e características únicas.

## 🏛️ Sistema "Integrando a Nação Brasileira" Expandido

**Requer DLC "Colossus of the South" (opcional)**

O mod agora **expande** o sistema vanilla de integração nacional do Brasil:

- Journal entry agora requer integração de **7 culturas** (4 vanilla + 3 novas)
- 3 novos botões de integração com requisitos únicos por cultura
- Sistema de heróis nacionais expandido - generais das novas culturas podem surgir em batalhas
- 3 eventos narrativos de integração únicos
- Sistema de radicalização inclui as novas culturas se falhar

**Requisitos de integração:**
- **Mineiro**: Fervor brasileiro > mineiro + (herói nacional OU minas de ouro nível 10+)
- **Carioca**: Fervor brasileiro > carioca + (herói nacional OU universidades/gov admin na capital)
- **Sertanejo**: Fervor brasileiro > sertanejo + (herói nacional OU ferrovias/fazendas no interior)

**Funciona sem DLC**: As culturas existem e funcionam normalmente, apenas o sistema de integração requer o DLC.

## 📜 4 Novos Eventos Históricos

- **Balaiada (1838-1841)** - Revolta popular no Maranhão com 3 opções de resolução
- **Sabinada (1837-1838)** - Movimento federalista na Bahia com 2 opções
- **Expansão do Café Fase 1 (1850+)** - Boom cafeeiro em São Paulo com 3 estratégias
- **Expansão do Café Fase 2 (1870+)** - Expansão para Minas Gerais e Rio de Janeiro

## 🌿 Traits Geográficas Brasileiras

- **Cerrado** - Savana brasileira (+10% agricultura, +15% ranching, -5% infraestrutura)
  - Aplicado em: Goiás, Tocantins, Mato Grosso, Mato Grosso do Sul
- **Caatinga** - Bioma semiárido único (-15% agricultura, -10% plantations, -10% migração)
  - Aplicado em: Ceará, Piauí, Rio Grande do Norte

## 🔧 Correções Críticas

- **Bug do Espírito Santo corrigido**: Estado não aparece mais branco/sem dono no mapa
- **Localizações corrigidas**: Todos os arquivos com namespace `l_braz_por` e UTF-8 com BOM
- **Traits traduzidas**: Cerrado e Caatinga aparecem com nomes corretos (não mais state_trait_...)

## ⚖️ Balanceamento

**Estados menores do Nordeste:**
- **Alagoas**: 80 → 120 terra arável, +10 ferro não descoberto, recursos aumentados
- **Sergipe**: 60 → 90 terra arável, +15 petróleo não descoberto, recursos aumentados

**Petróleo aumentado (v5.0):**
- São Paulo: 5 → 40 unidades
- Minas Gerais: 5 → 40 unidades
- Zulia (Venezuela): 60 → 120 unidades

**Terra arável balanceada (v5.0):**
- São Paulo: 220 → 160 (mais histórico para 1836)
- Pará: 400 → 120 (Amazônia não ideal para agricultura extensiva)

## 📊 Distribuição Cultural do Brasil

| Cultura | Estados | Vanilla/Mod |
|---------|---------|-------------|
| brazilian (paulista) | São Paulo | Vanilla |
| sulista | RS, SC, PR | Vanilla |
| nordestino | Nordeste | Vanilla |
| amazonic | Amazônia | Vanilla |
| **mineiro** | Minas Gerais | **MOD** |
| **carioca** | Rio de Janeiro | **MOD** |
| **sertanejo** | GO, TO, MT, MS | **MOD** |

## 📦 Instalação

1. Baixe o arquivo `.zip` abaixo
2. Extraia para `Documents/Paradox Interactive/Victoria 3/mod/`
3. Ative o mod no launcher do jogo

## ⚠️ Compatibilidade

- ✅ Victoria 3 versão 1.0+
- ✅ Funciona com ou sem DLC "Colossus of the South"
- ✅ Compatível com save games existentes
- ⚠️ Pode conflitar com mods que modificam o sistema cultural brasileiro

## 🆕 Arquivos Novos

**Culturas:**
- `common/cultures/00_brazilian_cultures.txt`
- `common/history/cultures/00_brazilian_cultures.txt`
- `localization/braz_por/cultures_l_braz_por.yml`

**Sistema de Integração Nacional:**
- `common/journal_entries/02_brazilian_nation_building.txt`
- `common/scripted_buttons/brazilian_culture_extended_buttons.txt`
- `events/brazil_culture_extended_events.txt`
- `events/culture_brazil_events_extended.txt`
- `localization/braz_por/brazilian_culture_extended_l_braz_por.yml`

**Eventos Históricos (v5.1):**
- `events/brazil_historical_events.txt`
- `common/modifiers/00_brazil_update_modifiers.txt`
- `localization/braz_por/events/brazil_events_l_braz_por.yml`

**Traits Geográficas (v5.1):**
- `common/state_traits/00_brazil_traits.txt`
- `localization/braz_por/map/traits_l_braz_por.yml`

## 🐛 Problemas Conhecidos

Nenhum conhecido até o momento. Reporte bugs na aba Issues do GitHub.

## 📝 Changelog Completo

Veja [CHANGELOG.md](CHANGELOG.md) para histórico completo de versões.

---

**Desenvolvido por**: metelrzx  
**Licença**: MIT
