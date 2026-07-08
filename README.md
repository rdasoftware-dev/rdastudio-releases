# RDAStudio IDE — Downloads e Releases

**rdastudio.com.br/download**

Repositório público para distribuição de binários, releases e changelog do **RDAStudio IDE**.

---

## Download

### Última versão estável

| Plataforma | Arquivo | Tamanho | Data |
| :--- | :--- | :--- | :--- |
| **Linux (x86_64)** | `rdastudio-linux-x86_64.tar.gz` | — | Em breve |
| **Linux (.deb)** | `rdastudio_0.1.0_amd64.deb` | — | Em breve |
| **Linux (AppImage)** | `rdastudio-0.1.0-x86_64.AppImage` | — | Em breve |

### Versão de desenvolvimento (nightly)

| Plataforma | Arquivo | Data |
| :--- | :--- | :--- |
| **Linux (x86_64)** | `rdastudio-nightly-linux-x86_64.tar.gz` | — |

---

## Instalação

### Linux (tar.gz)

```bash
tar -xzf rdastudio-linux-x86_64.tar.gz
cd rdastudio
./rdastudio
```

Linux (.deb)

```bash
sudo dpkg -i rdastudio_0.1.0_amd64.deb
rdastudio
```

Linux (AppImage)

```bash
chmod +x rdastudio-0.1.0-x86_64.AppImage
./rdastudio-0.1.0-x86_64.AppImage
```

---

Requisitos do sistema

Componente Mínimo
Sistema operacional Linux (Ubuntu 20.04+, Mint 21+, Debian 11+)
Arquitetura x86_64
Memória RAM 2 GB
Espaço em disco 500 MB
Dependências GTK3 (já incluso na maioria das distribuições)

---

Changelog

v0.1.0 (Em desenvolvimento)

· Editor de código com syntax highlighting Object Pascal
· Anotações de erro inline
· Compilação nativa Linux com um clique
· Cross-compilação para Windows
· Cross-compilação para Android
· Gerenciador de projeto simples
· Três templates: App Linux, App Windows, App Android

---

Verificação de integridade

Todos os binários são assinados com GPG. Para verificar:

```bash
gpg --verify rdastudio-linux-x86_64.tar.gz.sig rdastudio-linux-x86_64.tar.gz
```

Chave pública: [chave-gpg-aqui]

---

Links

🌐 Site oficial: rdastudio.com.br
📖 Documentação: rdastudio.com.br/docs
📧 Contato: contato@rdastudio.com.br
🏢 RDA Software: rdasoftware.com.br
💻 GitHub: github.com/rdasoftware-dev

---

Autor

Robson Dantas de Aguiar (RDA)
RDA Software
contato@rdasoftware.com.br
rdasoftware.com.br

---

Licença

O RDAStudio IDE é software proprietário. Consulte o arquivo LICENSE.txt incluído em cada distribuição para os termos completos. Componentes de terceiros são distribuídos sob suas respectivas licenças de código aberto (FPC, LCL, SynEdit, GTK3 — ver documentação).

```
