# Changelog

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

## [5.1] - 2024-10-13

### Adicionado
- **3 Novas Culturas Brasileiras**:
  - **Mineiro** (Minas Gerais) - Cultura focada na mineração e barroco colonial, obsessão: ouro
  - **Carioca** (Rio de Janeiro) - Cultura urbana cosmopolita da capital imperial, obsessão: móveis de luxo
  - **Sertanejo** (Centro-Oeste) - Cultura do interior seco, adaptada ao cerrado e sertão, obsessão: tecidos
- **Integração ao Sistema "Integrando a Nação Brasileira"** (requer DLC Colossus of the South):
  - 3 novos botões de integração cultural no journal entry
  - Heróis nacionais podem surgir das novas culturas em batalhas
  - Eventos de integração únicos para cada cultura nova
  - Requisitos específicos para integração (minas de ouro, infraestrutura capital, desenvolvimento do interior)
  - Sistema de radicalização se a integração falhar
- **Eventos Históricos Brasileiros**:
  - Balaiada (1838-1841) em Maranhão - revolta popular com 3 opções de resolução
  - Sabinada (1837-1838) na Bahia - movimento federalista com 2 opções
  - Expansão do Café em São Paulo (1850+) - evento de boom econômico com 3 estratégias
  - Segunda onda cafeeira (1870+) - expansão para Minas Gerais e Rio de Janeiro
- **Traits Geográficas Brasileiras**:
  - state_trait_cerrado - Savana brasileira (Goiás, Tocantins, Mato Grosso, Mato Grosso do Sul)
  - state_trait_caatinga - Bioma semiárido único do Brasil (Ceará, Piauí, Rio Grande do Norte)
- **14 Novos Modificadores** de eventos com efeitos balanceados
- **Recursos adicionados aos estados menores**:
  - Alagoas: +10 ferro não descoberto
  - Sergipe: +15 petróleo não descoberto
- Localização completa PT-BR para culturas, eventos, modificadores e traits

### Corrigido
- **Bug Crítico do Espírito Santo**: Estado aparecia branco/sem dono no mapa
  - Corrigida inconsistência de nomenclatura no arquivo de estados históricos
  - Estado agora pertence corretamente ao Brasil em 1836
- **Bug de Localização**: Namespace corrigido para `l_braz_por` em todos os arquivos
- **UTF-8 BOM**: Todos os arquivos de localização agora têm UTF-8 com BOM correto

### Alterado
- **Distribuição Cultural Atualizada**:
  - Minas Gerais agora usa cultura mineiro (antes brazilian)
  - Rio de Janeiro agora usa cultura carioca (antes brazilian)
  - Goiás, Tocantins, Mato Grosso e Mato Grosso do Sul agora usam cultura sertanejo
- **Sistema de Integração Nacional Expandido**:
  - Journal entry "Integrando a Nação Brasileira" agora requer integração de 7 culturas (antes 4)
  - Novas culturas podem gerar heróis nacionais através de vitórias militares
  - Evento de falha agora radicaliza todas as 7 culturas regionais
- **Balanceamento de Estados Menores do Nordeste**:
  - Alagoas: 80 → 120 terra arável, +3 capped resources, +10 ferro
  - Sergipe: 60 → 90 terra arável, +2 capped resources, +15 petróleo
- Cada cultura regional tem nomes próprios, sobrenomes e características únicas

### Arquivos Novos
- `common/cultures/00_brazilian_cultures.txt` - 3 novas culturas regionais
- `common/journal_entries/02_brazilian_nation_building.txt` - Journal entry expandido
- `common/scripted_buttons/brazilian_culture_extended_buttons.txt` - 3 botões de integração
- `events/brazil_culture_extended_events.txt` - 3 eventos de integração cultural
- `events/culture_brazil_events_extended.txt` - Eventos de heróis e falha expandidos
- `localization/braz_por/cultures_l_braz_por.yml` - Traduções das culturas
- `localization/braz_por/brazilian_culture_extended_l_braz_por.yml` - Traduções do sistema de integração
- `events/brazil_historical_events.txt` - 4 eventos históricos completos
- `common/modifiers/00_brazil_update_modifiers.txt` - 14 modificadores
- `common/state_traits/00_brazil_traits.txt` - 2 novas traits (Cerrado, Caatinga)
- `localization/braz_por/events/brazil_events_l_braz_por.yml` - Traduções dos eventos
- `localization/braz_por/map/traits_l_braz_por.yml` - Traduções das traits

## [5.0] - 2024-10-12

### Corrigido
- **Bug Crítico**: Corrigida nomenclatura inconsistente `STATE_ESP` → `STATE_ESPIRITO_SANTO` em todos os arquivos
- **Bug Crítico**: Corrigida província de mineração do Pará (x45DA42 estava no Amapá, alterado para x8839E0)
- Padronização de nomes de estados sem acentos nos IDs (mantendo acentos nas traduções)

### Alterado
- **Petróleo Aumentado**:
  - São Paulo: 5 → 40 unidades não descobertas
  - Minas Gerais: 5 → 40 unidades não descobertas
  - Zulia (Venezuela): 60 → 120 unidades não descobertas
- **Balanceamento de Terra Arável**:
  - São Paulo: 220 → 160 (mais histórico para 1836)
  - Pará: 400 → 120 (Amazônia não é ideal para agricultura extensiva)
- Descrição do mod atualizada com informações completas
- Tags adicionadas: Map, Historical, Brazil, Gameplay, Translation, Portuguese

### Mantido
- Minas Gerais mantido com ouro abundante (8 minas descobertas + 22 não descobertas)
- Terra arável de Minas Gerais mantida em 300 (maior estado agrícola)
- Todos os 8 novos estados brasileiros

## [4.x] - Versões Anteriores

### Adicionado
- 8 Novos estados brasileiros:
  - Espírito Santo (separado do Rio de Janeiro)
  - Alagoas (separado de Pernambuco)
  - Sergipe (separado de Pernambuco)
  - Amapá (separado do Pará)
  - Roraima (separado do Amazonas)
  - Rondônia (separado do Amazonas)
  - Tocantins (separado de Goiás)
  - Mato Grosso do Sul (separado de Mato Grosso)
- 2 Novos estados argentinos:
  - Entre Rios
  - Formosa
- Traits geográficas brasileiras:
  - state_trait_terra_roxa (São Paulo, Paraná)
  - state_trait_mata_atlantica (litoral sudeste)
  - state_trait_sertao (Bahia, nordeste)
  - state_trait_serra_dos_carajas (Pará)
- Tradução completa PT-BR de todos os estados do jogo
- População histórica detalhada para 1836
- Recursos naturais históricos:
  - Ouro em Minas Gerais
  - Ferro em várias regiões
  - Borracha na Amazônia
  - Petróleo (descoberto progressivamente)

### Modificado
- Rio de Janeiro dividido (8 províncias para RJ, 8 para Espírito Santo)
- Pernambuco dividido em três (PE, Alagoas, Sergipe)
- Amazonas dividido (Roraima, Rondônia)
- Pará dividido (Amapá separado)
- Recursos minerais aumentados em Minas Gerais
- Zulia (Venezuela) ganhou trait dos Andes

## Roadmap Futuro

### Planejado para v5.2
- [ ] Mais eventos históricos:
  - [ ] Abolição da Escravatura (1888)
  - [ ] Proclamação da República (1889)
  - [ ] Ciclo da Borracha - Amazonas
- [ ] Revisão de recursos dos novos estados:
  - [ ] Amapá: manganês (Serra do Navio)
  - [ ] Rondônia: cassiterita
  - [ ] Espírito Santo: portos melhorados
- [ ] Journal Entries específicos do Brasil

### Em Consideração
- Separar arquivo 00_states.txt em arquivos específicos por país
- Decisões customizadas para o Brasil
- Integração com eventos vanilla (Guerra do Paraguai, etc.)

## Notas de Desenvolvimento

### v5.1
Esta versão adiciona conteúdo dinâmico ao mod com eventos históricos que afetam o gameplay. Os eventos de café em São Paulo permitem ao jogador moldar o crescimento econômico do estado, enquanto os eventos de rebeliões regionais adicionam desafios históricos. As novas traits geográficas (Cerrado e Caatinga) tornam cada região do Brasil única com características próprias.

### v5.0
Esta versão foca em correções críticas e balanceamento baseado em feedback da comunidade. O foco principal foi corrigir bugs que poderiam causar crashes e ajustar valores econômicos para refletir melhor a realidade histórica de 1836, mantendo o jogo balanceado e divertido.

---

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/)
