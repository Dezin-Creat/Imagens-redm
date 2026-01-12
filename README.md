# Imagens RedM

Este repositório contém imagens de itens do **Red Dead Redemption Multiplayer (RedM)** para uso no framework **VORP**.

## 📋 Sobre

Estas são imagens de itens extraídas do RedM que podem ser utilizadas no sistema VORP para exibir ícones de itens no inventário, lojas e outras interfaces do servidor.

## 📁 Estrutura

```
Imagens-redm/
└── items/
    └── [arquivos .png]
```

A pasta `items/` contém todas as imagens dos itens em formato PNG, incluindo:
- Animais e peixes
- Munições
- Comidas e bebidas
- Roupas e acessórios
- Ferramentas e objetos diversos

## 🚀 Como Instalar no VORP

### Passo 1: Copiar as Imagens

Copie a pasta `items/` para o diretório de recursos do VORP. O caminho correto é:

```
vorp_inventory/html/img/items/
```

**Caminho completo de exemplo:**
```
resources/[vorp]/vorp_inventory/html/img/items/
```

### Passo 2: Verificar a Estrutura

Certifique-se de que a estrutura final fique assim:

```
vorp_inventory/
└── html/
    └── img/
        └── items/
            ├── a_c_animal_lobster_no_ped.png
            ├── ammo_box_pistol.png
            ├── apple_red.png
            └── ... (todas as outras imagens)
```

### Passo 3: Configurar os Itens

No arquivo de configuração dos itens do VORP (geralmente em `vorp_inventory/server/items.lua` ou similar), certifique-se de que os nomes dos arquivos de imagem correspondam aos nomes dos itens configurados.

**Exemplo:**
```lua
{
    name = "apple_red",
    label = "Maçã Vermelha",
    image = "apple_red.png",  -- Nome do arquivo na pasta items/
    -- ... outras configurações
}
```

### Passo 4: Reiniciar o Recurso

Após copiar as imagens, reinicie o recurso do inventário:

```
restart vorp_inventory
```

## ⚠️ Observações Importantes

- **Caminho Correto**: As imagens devem estar em `vorp_inventory/html/img/items/`
- **Formato**: Todas as imagens estão em formato PNG
- **Nomenclatura**: Os nomes dos arquivos devem corresponder exatamente aos nomes configurados nos itens do VORP
- **Case Sensitive**: Em sistemas Linux, os nomes dos arquivos são case-sensitive (maiúsculas/minúsculas importam)

## 📝 Notas

- Se alguma imagem não aparecer, verifique se o nome do arquivo corresponde exatamente ao nome configurado no item
- Certifique-se de que o servidor tem permissões de leitura na pasta de imagens
- As imagens podem ser redimensionadas pelo navegador, mas é recomendado manter um tamanho padrão (geralmente 64x64 ou 128x128 pixels)

## 🔗 Links Úteis

- [VORP Framework](https://github.com/VORPCORE)
- [RedM Documentation](https://docs.redm.gg/)

---

**Desenvolvido para uso com VORP Framework no RedM**