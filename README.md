# RDAStudio IDE

## Legal and Third-Party Notices

> **LEIA-ME ANTES DE TUDO:** Este documento não substitui aconselhamento jurídico profissional. Ele reflete o entendimento de boa-fé dos mantenedores do projeto sobre as licenças aplicáveis em 07 de julho de 2026. Em caso de dúvida legal, consulte um advogado especializado em propriedade intelectual.

---

## 1. Licenciamento do RDAStudio IDE

O código-fonte, a interface de usuário, a documentação original e os ativos visuais do **RDAStudio IDE** são propriedade intelectual de **Robson Dantas de Aguiar**, todos os direitos reservados.

- O uso do compilador Free Pascal (FPC) e da Lazarus Component Library (LCL) **não** torna o RDAStudio IDE um software de código aberto obrigatório.
- A distribuição dos binários compilados é regida pelos Termos de Serviço e pelo modelo de assinatura (Gratuito, Premium Standard, Premium Absoluto) definidos pela plataforma.

---

## 2. Componentes de Terceiros e Atribuições

O RDAStudio IDE é construído sobre os ombros de gigantes. As seguintes ferramentas e bibliotecas de código aberto são utilizadas:

### 2.1 Compilador e Ecossistema Base

| Componente | Licença | Uso no Projeto |
| :--- | :--- | :--- |
| **Free Pascal Compiler (FPC)** | GNU GPL v2+ (com exceção de compilação) | Compilador nativo e cruzado (Linux → Windows/Android). A exceção da GPL garante que os binários gerados não herdam a GPL. |
| **Lazarus Component Library (LCL)** | LGPL modificada (com exceção de linking estático) | Framework de interface gráfica da IDE. A exceção modificada permite linking estático e distribuição de binários proprietários. |

### 2.2 Componentes de Interface e Edição

| Componente | Licença | Uso no Projeto |
| :--- | :--- | :--- |
| **SynEdit** | MPL 1.1 (Mozilla Public License) | Base do editor de código customizado. Modificações no código-fonte do SynEdit permanecem sob MPL. |

### 2.3 Ferramentas de Pipeline e Distribuição

| Componente | Licença | Uso no Projeto |
| :--- | :--- | :--- |
| **Android NDK** | Apache 2.0 (Google) | Linkers e bibliotecas para cross-compilação ARM 64-bit. |
| **Android SDK Command Line Tools** | Apache 2.0 (Google) | Ferramentas mínimas de empacotamento (`aapt2`, `zipalign`, `apksigner`, `adb`). |
| **Gradle** | Apache 2.0 | Motor de montagem do APK. |
| **GTK3** | GNU LGPL v2.1 | Toolkit de widgets do sistema Linux. Linkado dinamicamente. |

---

## 3. Obrigações de Atribuição e Distribuição

### 3.1 O que o RDAStudio IDE DEVE fazer

- Incluir este arquivo (`LEGAL.md`) em todas as distribuições binárias.
- Exibir os créditos acima na tela "About" do aplicativo.
- Manter intactas as notas de copyright originais dos componentes de terceiros.

### 3.2 O que o RDAStudio IDE NÃO precisa fazer

- Abrir o código-fonte completo da IDE.
- Pagar royalties ou taxas de licenciamento aos projetos upstream.

### 3.3 Tela "About"

O texto mínimo da tela "About" deve conter:

> **RDAStudio IDE**  
> Free Pascal Development Environment for Linux  
> Autor: Robson Dantas de Aguiar (RDA)  
> rdastudio.com.br  
>  
> Este software utiliza:  
> Free Pascal Compiler (GPLv2+), Lazarus Component Library (LGPL modificada),  
> SynEdit (MPL 1.1), GTK3 (LGPLv2.1), Android NDK/SDK (Apache 2.0)

---

## 4. Propriedade Intelectual do Usuário Final

O RDAStudio IDE é uma ferramenta. Como tal:

- O código-fonte escrito pelo usuário é **100% propriedade do usuário**.
- Os binários gerados pelo pipeline de compilação são **100% propriedade do usuário**.
- O RDAStudio IDE não insere código proprietário, backdoors, ou telemetria oculta.

---

## 5. Contato para Questões Legais

- **E-mail (produto):** contato@rdastudio.com.br
- **E-mail (empresa):** contato@rdasoftware.com.br
- **Site:** rdastudio.com.br
- **GitHub:** https://github.com/rdasoftware-dev

---

*Este documento foi redigido em 07 de julho de 2026. Última revisão pendente de auditoria legal externa.*
```

---

README do repositório rdastudio-releases (com GitHub corrigido)

```markdown
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

· 🌐 Site oficial: rdastudio.com.br
· 📖 Documentação: rdastudio.com.br/docs
· 📧 Contato: contato@rdastudio.com.br
· 🏢 RDA Software: rdasoftware.com.br
· 💻 GitHub: github.com/rdasoftware-dev

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
