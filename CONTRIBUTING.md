# Contribuindo para Brazil Update +

Obrigado por considerar contribuir para o Brazil Update +! Este documento fornece diretrizes para contribuições.

## 🤝 Como Contribuir

### Reportando Bugs

Ao reportar um bug, inclua:

1. **Versão do mod** e **versão do Victoria 3**
2. **Descrição clara** do problema
3. **Passos para reproduzir** o bug
4. **Comportamento esperado** vs **comportamento atual**
5. **Screenshots/logs** se aplicável
6. **Lista de outros mods** que você está usando

### Sugerindo Melhorias

Sugestões são bem-vindas! Para propor melhorias:

1. Verifique se já não existe uma issue similar
2. Explique **por que** a mudança seria benéfica
3. Forneça **contexto histórico** se relevante
4. Considere o **impacto no balanceamento** do jogo

### Pull Requests

#### Antes de Submeter

1. Teste suas mudanças no jogo
2. Verifique se não quebrou funcionalidades existentes
3. Mantenha o estilo de código consistente
4. Atualize a documentação se necessário

#### Processo

1. Fork o repositório
2. Crie uma branch descritiva (`feature/novo-estado-acre`, `fix/bug-mineracao`)
3. Faça commits claros e descritivos
4. Push para sua branch
5. Abra um Pull Request

#### Convenções de Commit

```
feat: adiciona novo estado do Acre
fix: corrige bug de população em Salvador
docs: atualiza README com novos recursos
balance: ajusta recursos de petróleo em SP
```

## 📁 Estrutura do Projeto

```
mod/
├── common/
│   ├── history/
│   │   ├── pops/          # População dos estados
│   │   └── states/        # Configuração inicial dos estados
│   └── strategic_regions/ # Regiões estratégicas
├── localization/
│   └── braz_por/         # Traduções PT-BR
├── map_data/
│   └── state_regions/    # Definição dos estados
└── .metadata/            # Metadados do mod
```

## 🎨 Padrões de Código

### Nomenclatura de Estados

- **IDs**: Sem acentos, MAIÚSCULAS, underscore
  ```
  STATE_ESPIRITO_SANTO  ✅
  STATE_ESPÍRITO_SANTO  ❌
  ```

- **Traduções**: Com acentos e capitalização correta
  ```
  STATE_ESPIRITO_SANTO: "Espírito Santo"  ✅
  ```

### Formatação de Arquivos

- **Indentação**: 4 espaços (não tabs)
- **Encoding**: UTF-8 with BOM para arquivos de localização
- **Line Endings**: CRLF (Windows)

### Valores de Recursos

Mantenha o balanceamento histórico:

- **Terra Arável**: Base em dados históricos de capacidade agrícola
- **Minerais**: Reflita descobertas reais do século XIX
- **Petróleo**: `undiscovered_amount` para descobertas pós-1900
- **População**: Use censos históricos quando disponíveis

## 📚 Recursos Históricos

### Fontes Recomendadas

- Censos do IBGE (disponíveis a partir de 1872)
- "História Geral do Brasil" - Boris Fausto
- "Brasil: Uma História" - Eduardo Bueno
- Registros imperiais brasileiros (1822-1889)
- Atlas históricos do Brasil

### Dados de População (1836)

A população de 1836 é estimada por interpolação entre:
- Censo de 1811 (limitado)
- Censo de 1872 (primeiro censo nacional completo)

Sempre documente suas fontes nos comentários do código.

## 🧪 Testando

### Checklist de Testes

Antes de submeter um PR, teste:

- [ ] O jogo inicia sem crashes
- [ ] O mod aparece corretamente no launcher
- [ ] Estados aparecem no mapa com cores corretas
- [ ] População está distribuída corretamente
- [ ] Recursos aparecem quando descobertos
- [ ] Traduções aparecem corretamente em PT-BR
- [ ] Compatível com saves existentes (quando possível)
- [ ] Multiplayer sincroniza corretamente

### Teste em Jogo

1. Inicie uma nova campanha como Brasil
2. Verifique se todos os estados aparecem
3. Teste a construção de edifícios
4. Verifique se os recursos são descobertos corretamente
5. Jogue até 1860+ para testar eventos de longo prazo

## 🌍 Tradução

### Adicionando Novas Traduções

O mod atualmente suporta:
- Português Brasileiro (completo)

Para adicionar outros idiomas:

1. Crie `localization/{language}/map/states_l_{language}.yml`
2. Traduza todos os estados
3. Teste no jogo

## ⚖️ Balanceamento

### Filosofia de Design

- **Histórico primeiro**: Precisão histórica é prioridade
- **Jogabilidade equilibrada**: Não torne o Brasil OP
- **Progressão temporal**: Estados devem crescer ao longo do tempo
- **Diversidade regional**: Cada região deve ter características únicas

### Valores de Referência (1836)

| Estado | Terra Arável | População Aprox. | Recursos Principais |
|--------|-------------|------------------|---------------------|
| Minas Gerais | 300 | ~700k | Ouro, Ferro |
| São Paulo | 160 | ~300k | Café (futuro) |
| Rio de Janeiro | 90 | ~580k | Porto, Indústria |
| Bahia | ~200 | ~730k | Açúcar, Tabaco |
| Pará | 120 | ~140k | Borracha, Ferro |

## 🐛 Debugging

### Logs do Victoria 3

Logs estão em:
```
Documents/Paradox Interactive/Victoria 3/logs/
```

Procure por:
- `error.log` - Erros críticos
- `game.log` - Log geral do jogo

### Problemas Comuns

**Estados não aparecem no mapa**
- Verifique IDs em `strategic_regions`
- Confirme que províncias existem

**Crash ao carregar**
- Verifique encoding UTF-8 with BOM
- Procure por IDs duplicados
- Valide sintaxe dos arquivos

**População não aparece**
- Verifique `common/history/pops/`
- Confirme que culturas existem no jogo base

## 📞 Contato

- **Issues**: Para bugs e sugestões
- **Discussions**: Para perguntas gerais
- **Pull Requests**: Para contribuições de código

## 📜 Código de Conduta

- Seja respeitoso e construtivo
- Foque em melhorar o mod
- Aceite feedback de forma positiva
- Ajude outros contribuidores

## 📝 Licença

Ao contribuir, você concorda que suas contribuições serão licenciadas sob a mesma licença MIT do projeto.

---

Obrigado por ajudar a melhorar o Brazil Update +! 🇧🇷
