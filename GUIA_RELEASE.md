# Guia: Como Criar a Release v5.1 no GitHub

## Passo 1: Fazer Commit das Mudanças

```bash
# Adicionar todos os arquivos
git add .

# Fazer commit com a mensagem
git commit -F COMMIT_MESSAGE.txt

# Fazer push para o repositório
git push origin main
```

## Passo 2: Criar a Release no GitHub

### Opção A: Via Interface Web (Recomendado)

1. Acesse seu repositório no GitHub
2. Clique na aba **"Releases"** (lado direito)
3. Clique no botão **"Draft a new release"**
4. Preencha os campos:

**Tag version:**
```
v5.1
```

**Release title:**
```
Brazil Update+ v5.1 - Novas Culturas e Sistema de Integração Nacional
```

**Description:**
- Copie todo o conteúdo do arquivo `RELEASE_NOTES_v5.1.md`
- Cole na caixa de descrição

**Anexar arquivos (opcional):**
- Você pode criar um arquivo .zip do mod manualmente
- Ou deixar que os usuários baixem via "Download ZIP" do GitHub

5. Marque como **"Set as the latest release"** ✅
6. Clique em **"Publish release"**

### Opção B: Via Linha de Comando (com GitHub CLI)

Se você instalar o GitHub CLI (`gh`) futuramente:

```bash
# Criar tag
git tag v5.1

# Push da tag
git push origin v5.1

# Criar release
gh release create v5.1 \
  --title "Brazil Update+ v5.1 - Novas Culturas e Sistema de Integração Nacional" \
  --notes-file RELEASE_NOTES_v5.1.md
```

## Passo 3: Criar Arquivo ZIP do Mod (Opcional)

Se quiser anexar um arquivo .zip para download direto:

### No Windows:
1. Vá para a pasta do mod
2. Selecione todas as pastas/arquivos EXCETO:
   - `.git/`
   - `.gitignore`
   - `COMMIT_MESSAGE.txt`
   - `RELEASE_NOTES_v5.1.md`
   - Arquivos `.md` de documentação (opcional manter)
3. Botão direito → **"Enviar para" → "Pasta compactada"**
4. Renomeie para `brazil-update-plus-v5.1.zip`
5. Faça upload na release

### Via Git Bash:
```bash
# Criar arquivo zip excluindo arquivos desnecessários
git archive --format=zip --output=brazil-update-plus-v5.1.zip HEAD
```

## Passo 4: Publicar na Steam Workshop (Opcional)

Se quiser publicar na Steam Workshop do Victoria 3:

1. Abra Victoria 3
2. Launcher → Mods → "Upload Mod"
3. Selecione a pasta do mod
4. Preencha:
   - **Nome**: Brazil Update+ v5.1
   - **Descrição**: Use o conteúdo de `RELEASE_NOTES_v5.1.md`
   - **Changelog**: Use as notas da versão 5.1
   - **Tags**: Map, Historical, Brazil, Gameplay, Translation
5. Faça upload

## Resumo dos Arquivos Criados

✅ `COMMIT_MESSAGE.txt` - Mensagem de commit detalhada
✅ `RELEASE_NOTES_v5.1.md` - Notas da release formatadas
✅ Este guia - Instruções passo a passo

## Verificação Final

Antes de publicar, certifique-se:
- [x] Todos os arquivos foram commitados
- [x] CHANGELOG.md está atualizado
- [x] README.md reflete as novas funcionalidades
- [x] Sem menções a IA/Claude nos arquivos
- [x] Todos os arquivos de localização têm UTF-8 com BOM
- [x] Testado no jogo (opcional mas recomendado)

---

**Data da Release**: 2024-10-13
**Versão**: 5.1
